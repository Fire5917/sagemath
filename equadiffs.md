# Fiche : SageMath & Équations Différentielles

## Questions et Réponses

1. **Comment définir la fonction de l'équation différentielle \( E1 \) ?**  
   `function('Y')(t)`

2. **Comment définir la dérivée de l'équation \( E1 \) ?**  
   `diff(Y(t), t)`

3. **Comment résoudre l'équation différentielle \( E1 \) ?**  
   `desolve(diff(Y(t), t) + 2*Y(t) == cos(t), Y(t))`

4. **Comment ajouter une condition initiale \( y(0) = 1 \) ?**  
   `desolve(diff(Y(t), t) + 2*Y(t) == cos(t), Y(t), ics=[0, 1])`

5. **Que fait `eq_diff.substitute_function(Y, sol_ci)` ?**  
   Vérifie que la solution \( sol_ci \) satisfait l'équation \( eq_diff \).  
   Si c’est correct, retourne 0.

6. **Que représente la commande `plot_slope_field` ?**  
   Elle trace le champ de pente d’une équation différentielle.

7. **Comment indiquer \( y(0) = 0 \), \( y'(0) = 1 \) ?**  
   `desolve(diff(Y(x), x, 2) + 2*diff(Y(x), x) + Y(x) == 1 + x, Y(x), ics=[0, 0, 1])`

8. **Que représente la figure d’un champ de pente ?**  
   Elle montre les directions des tangentes aux solutions.

9. **Que fait `diff(x(t), t, 2)` ?**  
   Calcule la dérivée seconde de \( x(t) \).

10. **Caractérisation de \( x^2y' = (x-1)y \)**  
    - À coefficients variables  
    - Homogène  
    - D’ordre 1  
    - Linéaire
