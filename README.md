def interpolation_lineaire(x0, y0, x1, y1, x):
    # Formule d'interpolation linéaire
    y = y0 + ((y1 - y0) / (x1 - x0)) * (x - x0)
    return y

# Saisie des points (x0, y0) et (x1, y1)
x0 = float(input("Entrez x0 : "))
y0 = float(input("Entrez y0 : "))
x1 = float(input("Entrez x1 : "))
y1 = float(input("Entrez y1 : "))

# Saisie de la valeur à interpoler
x = float(input("Entrez la valeur de x : "))

# Calcul et affichage du résultat
resultat = interpolation_lineaire(x0, y0, x1, y1, x)
print("La valeur interpolée de y est :", resultat)
