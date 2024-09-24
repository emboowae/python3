import time

tik_tok = int(input("enter a number of seconds: "))  # enter some time to be calculated

for i in range(tik_tok,0,-1):  # iterate for every second
    seconds = int(i) % 60  # the seconds shouldn't exceed 60 seconds(% means modulus in math)
    minutes = int(i / 60) % 60  # minutes don't go above 60 minutes
    hours = int(i / 3600) % 24  # hours shouldn't exceed 24 hours
    days = int(i / 86400) % 7  # days shouldn't exceed 7 days
    weeks = int(i / 604800)
    time.sleep(1)  # time will delay by 1 second
    print(f"W{weeks:02} D:{days:02} H:{hours:02} M:{minutes:02} S:{seconds:02}")
    # outputs our results

