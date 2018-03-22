Router
==========
-  umožňuje navigaciu medzi komponentami

Výhody
==========
- načítanie dynamických parametrov z URL
- obmedzenie prístupu pre neautentifikovaných užívateľov

Základný router
==========
- potrebujeme Routes , RouterModule
- Routes - uloženie routrovania (cesta a dany komponent, na ktorý sa presmerujeme)

const nasRouter: Routes = [
    {path:"", redirectTo:"home", pathMatch:"full"}, //defualtna adresa
    {path:"home", component:HomeComponentComponent},
    {path:"red", component:RedComponent},
];

- RouterModule -  exportovanie naseho routru do modulu komponentu, v ktorom ho chceme pouzit

export const exportovanyModul = RouterModule.forRoot(nasRouter);

