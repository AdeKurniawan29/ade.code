import sys
import time


def jalanin_lirik():
    lirik = [
        ("I'll imagine we fell in love", 0.08),
        ("I'll nap under moonlight skies with you", 0.09),
        ("I think I'll picture us, you with the waves", 0.06),
        ("The ocean's colors on your face", 0.09),
        ("I'll leave my heart with your air", 0.09),
        ("So let me fly with you", 0.09),
        ("Will you be forever with me?", 0.15),
    ]

    delay = [0.2, 0.8, 0.8, 0.6, 1.2, 1.2, 1.1]
    print("\n Blue - Yung Kai")
    time.sleep(0.5)
    for i, (baris_lagu, delay_karakter) in enumerate(lirik):
        for karakter in baris_lagu:
            print(karakter, end='')
            sys.stdout.flush()
            time.sleep(delay_karakter)
        time.sleep(delay[i])
        print('')
    print("\n♡♡♡\n\n")
jalanin_lirik()
