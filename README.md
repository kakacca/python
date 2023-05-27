import time

def focus_timer(duration):
    print("开始专注\n")
    while duration > 0:
        mins, secs = divmod(duration, 60)
        timer = "{:02d}:{:02d}".format(mins, secs)
        print(timer, end="\r")
        time.sleep(1)
        duration -= 1

    print("时间到！")
