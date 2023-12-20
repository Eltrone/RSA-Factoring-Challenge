#!/usr/bin/env python3

def factorize(number):
    for i in range(2, number // 2 + 1):
        if number % i == 0:
            return i, number // i
    return number, 1

def process_file(filename):
    with open(filename, 'r') as file:
        for line in file:
            number = int(line.strip())
            p, q = factorize(number)
            print(f"{number}={p}*{q}")

if __name__ == "__main__":
    import sys
    if len(sys.argv) != 2:
        print("Usage: python factors.py <file>")
    else:
        process_file(sys.argv[1])
