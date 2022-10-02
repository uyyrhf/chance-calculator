#here type in the chance of it happening first attempt in %. for example 51.299 (without the %)
value = 1
#here type in the chance of it happening that satisfies you in %. for example 99.999 (also without the %)
good_amount = 99.999
anothervalue = value
some_variable = 100
attempt = 1

while value <= good_amount:
    print(f"Attempt {attempt}: {value}%")
    attempt += 1
    some_variable = 100 - value
    value = value + anothervalue * some_variable / 100

print(f"Attempt {attempt}: {value}%")
print("that's enough")
