from unittest.mock import sentinel
############### import
from tqdm import tqdm, trange
import time
import os
import wikipedia 
import colorama
from colorama import Fore, Back, Style
colorama.init()
################ Kezdő oldal
print (Fore.GREEN + "Számolás - 1")
print (Fore.RED + "Wiki - 2")
mi_legyem = input (Fore.CYAN + " > ")
if mi_legyem == ("1"):
    os.system('calc')
if mi_legyem == ("2"):
        wiki2 = input("mire szeretnél keresni?")
        
if wiki2 == wiki2:
    print (Fore.RED + 'keresés...')
    time.sleep(1)
    pbar = tqdm(total=100)
    for i in range(10):
        time.sleep(0.1)
        pbar.update(100)
        pbar.close()
    print (Fore.GREEN + 'Találat:')
    print ('\033[31m' + wikipedia.page(wiki2))
