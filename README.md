# gym-training-guide
#In this code you find a file writing code with the time
import datetime
def gettime():
    return datetime.datetime.now()

def take(k):
    if k==1:
        c=int(input("enter 1 for exercise & 2 for food"))
        if c==1:
            value=input("type here \n")
            with open("irfan_ex.py","a") as a :
                a.write(str([str(gettime())])+":"+value+"\n")
            print("successfully written")
        elif c==2:
            value = input("type here \n")
            with open("irfan_food.py", "a") as a:
                a.write(str([str(gettime())]) + ":" + value + "\n")
            print("successfully written")

    elif k==2:
        c = int(input("enter 1 for exercise & 2 for food"))
        if c == 1:
            value = input("type here \n")
            with open("afrin_ex.py", "a") as a:
                a.write(str([str(gettime())]) + ":" + value + "\n")
            print("successfully written")
        elif c == 2:
            value = input("type here \n")
            with open("afrin_food.py", "a") as a:
                a.write(str([str(gettime())]) + ":" + value + "\n")
            print("successfully written")
    else:
        print("please enter the valid input")
if __name__ == '__main__':
    print(take(1))
