def diagonalDifference(arr):
    prim_diag = sec_diag = 0

    for i in range(n):
        prim_diag += arr[i][i]
        sec_diag += arr[i][n-1-i]
    print(abs(prim_diag - sec_diag))



if __name__ == '__main__':
    n = int(input().strip())
    arr = []
    for _ in range(n):
        arr.append(list(map(int, input().rstrip().split())))

    diagonalDifference(arr)
