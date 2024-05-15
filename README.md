# Learn-Python
Learn python,games source by dea afrizal 

import random

welcome_message = "WELCOME TO KENTONS MINDGAMES!"
cinta_putrinuraini = 7

print("^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^")
print(f"** {welcome_message} **")
print("^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^")

nama_user = input("masukan nama kamu : ")


print(f"halo {nama_user}! Temukan cintamu,coba perhatikan kotak ini,manakah yang berisi hati putri ? |_| |_| |_| |_| |_| |_| |_| |_| |_| |_| ")

pilihan_user = int(input ("menurut kamu di kotak nomor berapa hati putri berada ? [1 / 2 / 3 / 4 / 5 / 6 / 7 / 8 / 9 / 10] : ")) #ketika kita memasukan angka validasi dengan tipe data string validasinya juga harus string,validasi ada di row 32

confirm_answer = input(f"kamu memilih {pilihan_user} apakah kamu yakin,hati putri ada disana [y/n] ?")  

if confirm_answer == "n":
    print("program di hentikan")
    exit()
elif confirm_answer == "y":
    if pilihan_user == cinta_putrinuraini:
        print(f"Selamat {nama_user} kamu benar !! hati putri ada di kotak nomor {cinta_putrinuraini} dan pilihanmu adalah kotak nomor {pilihan_user}")
    else:
        print(f"kamu SALAH! hati putri nuraini bukan berada di situ,tapi ada di kotak nomor {cinta_putrinuraini},sedangkan kamu memilih kotak nomor {pilihan_user} silahkan mencintai ulang,seharusnya jika cinta bisa merasakan keberadaan hatinya :p ")
else:
    print("silahkan mencintai ulang,seharusnya jika cinta bisa merasakan keberadaan hatinya :p")
    exit()
