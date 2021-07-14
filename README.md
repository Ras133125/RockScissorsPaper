# RockScissorsPaper
Добавте код в редактор и запустите. Игра Камень-Ножницы-Бумага

	import random
	hum_ch = True
	random_choice = ['r', 's', 'p']

	while hum_ch:
   	 print('Камень - Ножныци - Бумага')
   	 print('Камень - Rock - R \nНожницы - Scissors - S \nБумага - Paper - P')
    	computer_random = random.choice(random_choice)
    	#print(computer_random)
    	human_random = input('R или S или P - ').lower()
   	 if human_random not in ['r', 's', 'p']:
        	print('------------')
        	print('Неверный ввод. Попробуйте следовать инструкции.')
        	print('------------')
        	continue
    
    
    
    	if computer_random == human_random:
        	print('Вы равны по силе!')
    
    	if computer_random == 'r' and human_random == 's': #камень-ножницы
        	print('Камень бьёт ножницы - Вы проиграли')
    	elif computer_random == 's' and human_random == 'r':
        	print('Камень бьёт ножницы - Вы выиграли')
   
    	if computer_random == 's' and human_random == 'p': #ножницы-бумага
        	print('Ножницы режут бумагу - Вы проиграли')
    	elif computer_random == 'p' and human_random == 's':
        	print('Ножницы режут бумагу - Вы выиграли')
    
    	if computer_random == 'p' and human_random == 'r': #бумага-камень
        	print('Бумага оборачивает камень - Вы проиграли')
    	elif computer_random == 'r' and human_random == 'p':
        	print('Бумага оборачивает камень - выиграли')
    
    
    	print('Хотите ещё?')
    	human_answer = True
    	while human_answer:
        	human_choice = input('Да(Y) или Нет(N)').lower()
        	if human_choice not in ['y', 'n']:
            	print('------------')
            	print('Неверный ввод. Попробуйте следовать инструкции')
            	print('------------')
            	continue
        	else:
            	break
    
    
    	if human_choice == 'y':
        	print('----------\n----------')
        	continue
    	if human_choice == 'n':
        	break

        
	print('Спасибо за игру!')
    
