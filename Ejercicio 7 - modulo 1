def esprimo(n, numprimos):

    if n < 2:
        return False
    for p in numprimos:
        if p * p > n:
            break
        if n % p == 0:
            return False
    return True

def intervalonoprimos(x):

    primernum = 4
    numprimos = [2, 3]
    while True:
        noprimos = 0
        for i in range(primernum, primernum + x):
            if esprimo(i, numprimos):
                break
            noprimos += 1
        if noprimos == x:
            return (primernum, primernum + x -1)
        primernum += 1
        for i in range(numprimos[-1] + 1, primernum + 10):
            if esprimo(1, numprimos):
                numprimos.append(i)

intervalo = intervalonoprimos(73)

print(f"Intervalo de {intervalo[0]} a {intervalo[1]}")
