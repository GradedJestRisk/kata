https://www.youtube.com/watch?v=nbSaq_ykOl4

Pour une série [1; N] avec N <= 100
- si N est divisible par 3, renvoyer Fizz ( N mod 3 = 0 => Fizz)
- si N est divisible par 5, renvoyer Buzz
- si N est divisible par 15, renvoyer FizzBuzz
- sinon renvoyer N

[ 1; 20]
12FizzBuzzFizz78FizzBuzz11Fizz1314FizzBuzzFizz17Fizz19Buzz

Contraintes:
- Sans debugger
- TCR
- Moins de 10 minutes la deuxième fois

Paradigme
- procédural
- fonctionnel
- orienté-objet

Step 0: 
- tester la lib - false puis true
- split screen code/test
- test case list shopping
- choose item in list

Step 1 : un seul nombre

N = 
- 1 : fake it return 1 (pas de paramètre)  
- 2: early exit pour 1 + refactor return(N) + refactor code de test si OOP ?
- 3: early exit =3 Fizz
- 6: early exit =3 ou =6 Fizz (triangulation) 
- refactor early exit mod 3 + refactor test context
- 5: ajout early exit = 5 
- 10 :  ajout early exit = 5 ou 10
- refactor early exit mod 5
- 15: ajout early exit 15
- 30: ajout early exit = 15 ou 30
- refactor early exit mod 15

Step 2 : une série de 2 nombres 

- [1,2] => '12' : ajout test + ajout param pour bornes + modif de tous les tests  avec inf = sup + fake it ?
- refacto nom des paramètres (min et max)
- plutot que return, utiliser +=  et dupliquer min et max + rajouter une guard clause bloc 2 si min = max
- extract function 

Step 3 : une série de 3 nombres

- [ 1, 2, 3] => '12Fizz': transformer le if en while avec compteur (ou mutation de paramètres ? tester pré ou post incrémentation)
- extract function sur le while

Step 3 : une série de x nombres
- [ 1; 15] et muter l'implémentation
