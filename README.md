# objects
Standard objects for API, View, Controller. API Definition files can be used to create stubs in popular languages, like Java, Scala, and Ruby, with just a few clicks.

## Definicje produktu, finalne wersje

+ Marketing produktu/uslugi

      + strona www projektu dla klientow, do zakupu, inne adresy stron
      + logo
      + profile spolecznosciowe
      + oferta
      + metody dystrybucji
      
+ Kod zrodlowy oproduktu/uslugi

      + repozytorium

+ Dokumentacja wedle ktorej byl tworzony produkt

      + repozytorium, wiki, 
      + unitAPI
      
## Definicje srodowiska, dokumentacja, narzedzia  Dev Tools

+ vodAPI.com - describe environment, definition of environment, zarzadzanie srodowiskiem pozwalajacym na realizacje projektu

      + jakie technologie beda uzyte w projekcie ?
      + jakie metody zarzadzania?
      + opis stanowiska pracy dla kazdego uczestnika projektu, 
            jakie opgrogramowanie i sprzet jest potrzebne
            + gitlab / github / bitbucket ?             
      + jakie metody komunikacji?
            + dla dev, customers, testers, ...
      + jakie stanowiska
      + jakie etapy w realizacji zlecenia
      + scenariusze, schematy, przyklady realizacji
      
Przyklady uzycia: 
      
      + opisywanie uslug firmy jako moduly, gdzie kazdy rodzaj uslugi ma specyfikacje oraz droge sprzedazy i wsparcia
      + standardy komunikacji, okreslenie kazdego dzialania jakie jest w realnym swiecie realizowane w trakcie
      + opsywanie tych dzialan kodem w jeyzku python, gdyz potem mozna uzyc te modele do utworzenia modeli do uczenia maszynowego
      + opisywanie scenariuszy jakie mialy miejsce i bazujac na juz zdobytych doswiacdczeniach budowanie lepszych scenariuszy, efektywniejszych
      + budowanie jak najmniejszych modulow z punktu widzenia efektywnosci sprzedazy i wspolpracy
      + proba utworzenia jak najmniejszych modulow z juz istniejacych
      + tworzenie API w aplikacjach pomagajacych na dostep do danych

Przyklady zapisu dokumentacji:

      project:
      + name: "projekt i wykonanie graficznego logotypu"
      + description: "How to create logo"
      + tags: Logo Creating, logo

      resources:      
      + positions: 
            + "Projektant"
            + "Grafik"
            + "Konsultant"
            + "Ksiegowa"
      + "Marketing/Budget/Money": 200EUR
      + "estimation": 12days    
      
      
      variables:
            Money
                  + zaliczka - kwota na poczatku zlecenia
                  + reszta - suma pozostala
                  + dodatkowe - koszty 
            Doc
                  + specyfikacja
                  + poprawki
                  + przedwykonaniem
                  + powykonawcza
            
            Produkt
                  + prototyp
                  + poprawiony
                  + finalny
            Status
                  + poprawny
                  + do poprawki
                  + 
            Klient, Producent
                  + Create
                  + Read
                  + Valid
                  + Update
                
      
      process:
            Klient
                  Create: Doc.specyfikacja
            Producent
                  Read: Doc.specyfikacja
                  Create: Produkt.prototyp
            Klient                  
                  Read: Produkt.prototyp
                  // result Boolean
                  if(Valid: Produkt.prototyp)                        
                        Update: Status.poprawny
                  else
                        Create: Doc.poprawki
                        Update: Status.do_poprawy
            
            Producent
            if(Valid: Produkt.prototyp && Update: Status.poprawny){
            
      
      // 1 Etap
      Projektant.wykonaj(dokumentacja.specyfikacja, Money.zaliczka) {
            dokumentacja // wszystkie informacje dotyczace rozpoczecia i zakonczenia pracy
      }
      
Przyklad programista


      Test-Driven Development (TDD).

      This is how it works:

          Write a test. – The test will flesh out some functionality in your app
          Then, run the test – The test should fail, since there's no code to make it pass.
          Write the code – To make the test pass
          Run the test – If it passes, you are confident that the code you've written meets the test requirements
          Refactor code – Remove duplication, prune large objects and make the code more readable. Re-run the tests every time you refactor the code
          Repeat – That's it!



+ APIcra.com - create scripts to create described environment, DevOpsTool

      + skrypty do uzycia w konsoli
      + install
      + create mysql
      + deploy
      
+ unitAPI.com - describe units in project, architecture of code, modules, zarzadzanie tworzeniem nowego kodu
[Backend.md](Backend.md)
      + zanim zostana zdefiniowane detale konieczne jest stworzenie prototypu, czyli wersji 0.0.1 ...
      + realizacja kolejnych wersji oprogramowania wraz z dokumentacja na kazdym etapie
      + wytyczne dla tworzenia standardow w aplikacji, dla programistow tworzacych kolejne moduly, 
            np na zamowienie

+ DevOpsTerminal, DevOpsTool

      + uzywa skryptow apicra
      + komunikacja z serwerem i zespolem poprzez chat tekstowy, 
            mozliwosc integracji z systemem zarzadzania repozytorium
      


... more info 
https://blog.devtoolsbox.com/index.php/2018/11/08/nowe-narzedzia-dla-devops-team-apicra-unitapi-vodapi/

## Tools API
Codegen

https://github.com/swagger-api/swagger-codegen-generators

