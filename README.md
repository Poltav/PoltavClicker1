#tapper.coin.meaning
sdf = 0

#slot
slot1 = 'none'
slot2 = 'none'
slot3 = 'none'

#promocode
promocode = input("Введите промокод , есле его нет введите '1'")
if promocode == "8800555600700":
    sdf = 10000
elif promocode == "96964545232":
    slot1 = "Xegor"
elif promocode == "1234567890":
    sdf = 10
elif promocode == 1:
    sdf = 0
else:
    print('Не найдено')
    sdf = 0

#start.prt
print('')

#tap.meaning
tap = 'q'

#clicker
while tap != 'del:code:cache':
    tap = input(sdf)
    sdf += 1

    #tap.command
    if tap == '/b':

        #shop
        bm = input('1 - Xegor(100)  2 - Vedasfer(1000)   3 - Colabed(10000)')
        if bm == "1" and sdf >= 100:
            slotchacker = input('1 - 1слот . 2 - слот . 3 - 3слот')
            if slotchacker == "1":
                sdf -= 100
                slot1 = ('Xegor')
            if slotchacker == "2":
                sdf -= 100
                slot2 = ('Xegor')
            if slotchacker == "3":
                sdf -= 100
                slot3 = ('Xegor')
        if bm == "2" and sdf >= 1000:
            slotchacker = input('1 - 1слот . 2 - слот . 3 - 3слот')
            if slotchacker == "1":
                sdf -= 1000
                slot1 = ('Vadesfer')
            if slotchacker == "2":
                sdf -= 1000
                slot2 = ('Vadesfer')
            if slotchacker == "3":
                sdf -= 1000
                slot3 = ('vadesfer')
        if bm == "3" and sdf >= 10000:
            slotchacker = input('1 - 1слот . 2 - слот . 3 - 3слот')
            if slotchacker == "1":
                sdf -= 10000
                slot1 = ('Colabed')
            if slotchacker == "2":
                sdf -= 10000
                slot2 = ('Colabed')
            if slotchacker == "3":
                sdf -= 10000
                slot3 = ('Colabed')

    #tap.command    
    if tap == '/slot1':
        print(slot1)
    if tap == '/slot2':
        print(slot2)
    if tap == '/slot3':
        print(slot3)
    if tap == '/profile':
        print('Очки',sdf)
        print('слоты:',slot1,",",slot2,',',slot3)
