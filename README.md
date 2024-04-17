def fibonacci(n):
   
    fib_sequence = [0, 1]

  
    for i in range(2, n):
        next_fib = fib_sequence[-1] + fib_sequence[-2]
        fib_sequence.append(next_fib)

    return fib_sequence


n = int(input("Enter the number of terms: "))


if n <= 0:
    print("Please enter a positive integer.")
else:
   
    fib_sequence = fibonacci(n)
    print("Fibonacci sequence up to", n, "terms:", fib_sequence)
