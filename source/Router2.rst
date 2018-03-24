Router 
=============

Guards - canActivate()
=============
- obmedzenie prístupu používateľa ku danej komponente

- vygenerovanie si guard:  ng g guard  ./guards/LoggedIn

- funkcia canActivate -> vracia true, ak ma pouzivatel pristup

//Guards
 if(localStorage['logged'] == "true"){
      return true;
    } else {
      this.router.navigate(['./KomponentNoAccess']); //komponent s chybovou hlaskou, ze nemame pristup
    }
    
 //Router
 
 {path:"red", component:RedComponent, canActivate:[NazovGuard]},
 
 //App.module.ts
 pridame nase guards do providers
 
 @NgModule({
     providers: [LoggedInGuard],
})
 
 


