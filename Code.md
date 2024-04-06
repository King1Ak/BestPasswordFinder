import datetime as dt
   
"ex:⇩"
Password = 986734

def crack_password():
    start = dt.datetime.now()
    for n in range(1000000):
        password_guess = '{0:04d}'.format(n)
        if password_guess == str(Password):
            end = dt.datetime.now()
            print("Password found: {} in {}".format(password_guess, end - start))
            break
    guesses = crack_password()

print(crack_password())
