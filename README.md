# hello-world chose your own adventure
This is my first project I have 2 days of studies but had learned some coding a while back. This project is for a simple text based game with multiple chose


print("Wellcome To The Wold of Dragons land")
name = input("What is your name traveler? ")
print(name,"I see,  the mane of a mity worrior.")
age = int(input("what is your age worrior? "))



if age >= 18:
  print ("Your are old enough")
  wants_to_play = input("do you want to play (Yes/No)? ").lower()

  health = 10
  print ("Your health is ", health, "do not wast it")

  if wants_to_play == "yes":
    print ("Lets Play! ")
    left_or_right = input("First chice... Left or right(Left/right)?")
    
    if left_or_right == "left":
      ans = input("Nice, you fallow the path and reach a lake... Do you swim across or go raund it (across/around)? ")
      
      if ans == "around":
        print ("you whent around and reached the other side of the lake. ")
      
      elif ans == "across":
        print ("You manage to get across, but were bit by a creature of the deep and lost 5 health. ")
        health -= 5

      ans = input ("you notice a house and a rive which do you go to (house/river)? ")

      if ans == "house":
        print ("As you enter the house a shadowy figure attacks you from behind. you lose 5 healt ")
        health -= 5
        if health <= 0:
          print ("you have 0 healt, you lost ")
        else:
          print ("You have survive you win")
        
      else:
        print ("you fell in the river and drown. you lost ")


    else:
      print ("You fall on a hold and die. ")


  else:
   print("cya... ")

elif age >= 14:
  print ("You can play with a older aventurer", name)

  secon_player_age = int(input ("how old in you your companian "))
  if secon_player_age >= 18:
    print ("you can prosid with your quest")
  else:
    print ("you shal not continue any farter")

else:
    print ("you shal not continue any farter")
