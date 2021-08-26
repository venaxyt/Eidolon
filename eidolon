# Made by @venaxyt on Github
import threading, requests, gratient, random, string

banner = """
   ▄███▄   ▄█ ██▄   ████▄ █    ████▄    ▄   
   █▀   ▀  ██ █  █  █   █ █    █   █     █  
   ██▄▄    ██ █   █ █   █ █    █   █ ██   █ 
   █▄   ▄▀ ▐█ █  █  ▀████ ███▄ ▀████ █ █  █ 
   ▀███▀    ▐ ███▀            ▀      █  █ █ 
                    v  e  n  a  x    █   ██ 
"""

print(gratient.purple(banner))
image_directory = "C:\\Users\\%username%\\Desktop\\images"

def FREEIMAGEHOST():
    while True:
        image_code = "".join(random.choice(string.ascii_uppercase + string.digits + string.ascii_lowercase) for _ in range(6))
        FREEIMAGEHOST_image_link = f"https://iili.io/{image_code}.png"
        FREEIMAGEHOST_image = requests.get(FREEIMAGEHOST_image_link)
        if FREEIMAGEHOST_image.status_code == 200:
            print(gratient.blue(f"   [>] FREEIMAGEHOST : {FREEIMAGEHOST_image_link}"), end = "")
            FREEIMAGEHOST_image_download = requests.get(FREEIMAGEHOST_image_link)
            open(f"{image_directory}\\{image_code}.png", "wb").write(FREEIMAGEHOST_image_download.content)
            #    v    e    n    a    x
threading.Thread(target = FREEIMAGEHOST).start(); threading.Thread(target = FREEIMAGEHOST).start(); threading.Thread(target = FREEIMAGEHOST).start(); threading.Thread(target = FREEIMAGEHOST).start()
