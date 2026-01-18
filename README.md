# Chatbot-with-Python
import datetime
import math
import random
def date():
    x=datetime.date.today()
    return(x.strftime("%x"))

def time():
    y=datetime.datetime.now()
    return(y.strftime("%X"))

def weekday():
    w=datetime.datetime.now()
    return(w.strftime("%A"))

def day_of_year():
    d=datetime.datetime.now()
    return(d.strftime("%j"))

def arethematic_op(x):
    if"add" in x:
        a=int(input("Enter the number :"))
        b=int(input("Enter the other number :"))
        c=a+b
        return(c)
        
    elif"subtract" in x:
        a=int(input("Enter the number :"))
        b=int(input("Enter the other number :"))
        c=a-b
        return(c)
    elif"multiply" in x:
        a=int(input("Enter the number :"))
        b=int(input("Enter the other number :"))
        c=a*b
        return(c)
    elif"divide" in x:
        a=int(input("Enter the number :"))
        b=int(input("Enter the other number :"))
        c=a/b
        return(c)

def maths(x):
    if "squareroot" in x:
        a=int(input("Enter the number :"))
        r=math.sqrt(a)
        return(round(r,4))
    elif "cuberoot" in x:
        a=int(input("Enter the number :"))
        if(a>0):
            r=math.pow(a,1/3)
            return(round(r,4))
        else:
            r=(-(math.pow(-a,1/3)))
            return(round(r,4))
    elif "exponent" in x or "power of" in x:
        a=int(input("Enter the number :"))
        p=int(input("Enter the power :"))
        if(a>0):
            r=math.pow(a,p)
            return(round(r,4))
        else:
            r=(-(math.pow(-a,p)))
            return(round(r,4)) 

def log(x):
    if "log with base 10" in x:
        l=int(input("Enter the number :"))
        r=math.log10(l)
        return(round(r,7))
    else:
        l=int(input("Enter the number :"))
        b=int(input("Enter the base number :"))
        r=math.log(l,b)
        return(round(r,7)) 

def dicex():
    v=random.randint(1,6)
    print(v)
    return()
def dice():
    while(True):
        dicex()
        c=input("To stop enter 's'")
        if "s" in c.lower():
            break
        else:
            continue

def coinx():
    c=["Heads","Tails"]
    r=random.choice(c)
    print(r)
    return()  
def coin():
    while(True):
        coinx()
        c=input("To stop enter 's'")
        if "s" in c.lower():
            break
        else:
            continue   

def rpsx():
    c=["Rock","Paper","Scissors"]
    r=random.choice(c)
    print(r)
    return()  
def rps():
    while(True):
        rpsx()
        c=input("To stop enter 's'")
        if "s" in c.lower():
            break
        else:
            continue    

def num():
    x=int(input("Enter the range :"))
    v=random.randint(1,x)
    print(v)
    return()
def pick_a_num():
    while(True):
        num()
        c=input("To stop enter 's'")
        if "s" in c.lower():
            break
        else:
            continue

def animalx():
    c= [
    "Tiger", "Lion", "Elephant", "Giraffe", "Zebra", 
    "Cheetah", "Leopard", "Gorilla", "Chimpanzee", "Bear", 
    "Dog", "Cat", "Horse", "Cow", "Pig", 
    "Sheep", "Goat", "Chicken", "Donkey", "Rabbit", 
    "Eagle", "Owl", "Penguin", "Peacock", "Parrot", 
    "Whale", "Dolphin", "Shark", "Octopus", "Jellyfish", 
    "Crocodile", "Alligator", "Chameleon", "Iguana", "Komodo Dragon", 
    "Rhinoceros", "Hippopotamus", "Kangaroo", "Panda", "Wolf", 
    "Fox", "Deer", "Moose", "Bison", "Camel", 
    "Hyena", "Koala", "Sloth", "Orangutan", "Raccoon", 
    "Skunk", "Otter", "Beaver", "Platypus", "Wombat", 
    "Meerkat", "Hedgehog", "Squirrel", "Bat", "Lemur", 
    "Ostrich", "Flamingo", "Swan", "Duck", "Goose", 
    "Turkey", "Woodpecker", "Hummingbird", "Hawk", "Falcon", 
    "Vulture", "Pigeon", "Seagull", "Pelican", "Kingfisher", 
    "Sea Lion", "Walrus", "Seal", "Orca", "Stingray", 
    "Seahorse", "Crab", "Lobster", "Shrimp", "Starfish", 
    "Squid", "Eel", "Salmon", "Tuna", "Clownfish", 
    "Turtle", "Tortoise", "Cobra", "Rattlesnake", "Frog", 
    "Toad", "Butterfly", "Bee", "Ant", "Spider"]
    r=random.choice(c)
    print(r)
    return()  
def animals():
    n=int(input("Enter how many you want :"))
    a=1
    while(a<=n):
        animalx()
        a+=1
    print("Thats all! I have provided you with ", n," animals") 

def colorx():
    c=[
    "Red", "White", "Cyan", "Blue", "Black", "Yellow", "Pink", "Orange", "Magenta", "LightBlue",
    "Lime", "Gold", "DarkBlue", "Green", "Purple", "Silver", "Gray", "Aquamarine", "Maroon", "Azure Blue",
    "Red Blood", "Blue Gray", "Black Blue", "Sage Green", "Wood", "Night", "Isle Of Man Green", "Neon Yellow", "Millennium Jade", "Brown",
    "WhiteSmoke", "Light Red", "Olive", "Metallic Silver", "Bronze", "Crimson", "Light Purple Blue", "Light Black", "Night Blue", "Metallic Gold",
    "Dark White", "LightYellow", "Windows Blue", "Navy", "DarkGreen", "Beige", "Bright Gold", "Warm White", "Red Gold", "White Gold",
    "Neon Pink", "DeepSkyBlue", "Love Red", "Neon Purple", "White Gray", "HotPink", "Saffron Red", "SkyBlue", "LightGreen", "Indigo",
    "Silver White", "Orchid Purple", "Off White", "Neon Orange", "Dark Beige", "Teal", "Midnight Purple", "Golden Blonde", "LightGray", "Deep Yellow",
    "Neon Gold", "Dark Gold", "Charcoal", "Milk White", "Neon Red", "Dark Bronze", "DarkOrange", "Iron Gray", "Pearl White", "Caramel",
    "Oil", "Deep Purple", "Cream White", "Bronze Gold", "Stormy Gray", "Lavender Purple", "Ferrari Red", "Blonde", "Bright Teal", "Turquoise",
    "DodgerBlue", "Golden Yellow", "Champagne Gold", "Salmon", "Chocolate", "Coral", "Fuchsia", "Ivory", "Khaki", "Lavender"]
    r=random.choice(c)
    print(r)
    return()
def color():
    n=int(input("Enter how many you want :"))
    a=1
    while(a<=n):
        colorx()
        a+=1
    print("Thats all! I have provided you with ", n," colours")    

def peoplex():
    c=[
    "Narendra Modi", "Mukesh Ambani", "Virat Kohli", "Shah Rukh Khan", "Amitabh Bachchan",
    "Gautam Adani", "Ratan Tata", "Mahendra Singh Dhoni", "Deepika Padukone", "Alia Bhatt",
    "Salman Khan", "Akshay Kumar", "Priyanka Chopra Jonas", "Rohit Sharma", "Sachin Tendulkar",
    "S.S. Rajamouli", "Aamir Khan", "Ranbir Kapoor", "Ranveer Singh", "Hrithik Roshan",
    "Droupadi Murmu", "Amit Shah", "Rahul Gandhi", "Mamata Banerjee", "Yogi Adityanath",
    "Arvind Kejriwal", "Nitin Gadkari", "S. Jaishankar", "Ajit Doval", "Nirmala Sitharaman",
    "Anand Mahindra", "Shiv Nadar", "N.R. Narayana Murthy", "Kiran Mazumdar-Shaw", "Azim Premji",
    "Uday Kotak", "Sunil Mittal", "Falguni Nayar", "Cyrus Poonawalla", "Radhakishan Damani",
    "Neeraj Chopra", "P.V. Sindhu", "Hardik Pandya", "Shubman Gill", "Suryakumar Yadav",
    "Rishabh Pant", "Jasprit Bumrah", "Sunil Chhetri", "Mary Kom", "Mirabai Chanu",
    "Rajinikanth", "Kamal Haasan", "Joseph Vijay", "Ajith Kumar", "Prabhas",
    "Allu Arjun", "Mahesh Babu", "N.T. Rama Rao Jr.", "Ram Charan", "Yash",
    "Mohanlal", "Mammootty", "Fahadh Faasil", "Nayanthara", "Samantha Ruth Prabhu",
    "Rashmika Mandanna", "Kiara Advani", "Shraddha Kapoor", "Kriti Sanon", "Triptii Dimri",
    "Kartik Aaryan", "Vicky Kaushal", "Katrina Kaif", "Kareena Kapoor Khan", "Aishwarya Rai Bachchan",
    "Kajol", "Vidya Balan", "Taapsee Pannu", "Ayushmann Khurrana", "Rajkummar Rao",
    "Manoj Bajpayee", "Pankaj Tripathi", "Nawazuddin Siddiqui", "Anupam Kher", "A.R. Rahman",
    "Lata Mangeshkar", "Arijit Singh", "Sonu Nigam", "Shreya Ghoshal", "Diljit Dosanjh",
    "Badshah", "CarryMinati (Ajey Nagar)", "Bhuvan Bam", "Ashish Chanchlani", "Ranveer Allahbadia",
    "Sundar Pichai", "Satya Nadella", "Kailash Satyarthi", "Amartya Sen", "Sania Mirza"]
    r=random.choice(c)
    print(r)
    return() 
def people():
    n=int(input("Enter how many you want :"))
    a=1
    while(a<=n):
        peoplex()
        a+=1
    print("Thats all! I have provided you with ", n," peoples")

def placex():
    c=[
    "New York City, USA", "London, UK", "Paris, France", "Tokyo, Japan", "Sydney, Australia",
    "Rome, Italy", "Rio de Janeiro, Brazil", "Beijing, China", "Dubai, UAE", "Cairo, Egypt",
    "Mumbai, India", "Cape Town, South Africa", "Moscow, Russia", "Berlin, Germany", "Toronto, Canada",
    "Mexico City, Mexico", "Istanbul, Turkey", "Bangkok, Thailand", "Seoul, South Korea", "Singapore",
    "Great Wall of China", "Eiffel Tower", "Statue of Liberty", "Colosseum", "Taj Mahal",
    "Pyramids of Giza", "Machu Picchu", "Christ the Redeemer", "Petra", "Chichen Itza",
    "Mount Everest", "Amazon Rainforest", "Sahara Desert", "Great Barrier Reef", "Victoria Falls",
    "Grand Canyon", "Niagara Falls", "Mount Fuji", "The Alps", "The Himalayas",
    "Vatican City", "Las Vegas, USA", "Venice, Italy", "Barcelona, Spain", "Amsterdam, Netherlands",
    "Prague, Czech Republic", "Vienna, Austria", "Athens, Greece", "Dublin, Ireland", "Stockholm, Sweden",
    "Copenhagen, Denmark", "Helsinki, Finland", "Oslo, Norway", "Zurich, Switzerland", "Lisbon, Portugal",
    "Warsaw, Poland", "Budapest, Hungary", "Kuala Lumpur, Malaysia", "Ho Chi Minh City, Vietnam", "Manila, Philippines",
    "Jakarta, Indonesia", "Hanoi, Vietnam", "Istanbul, Turkey", "Buenos Aires, Argentina", "Santiago, Chile",
    "Lima, Peru", "Bogota, Colombia", "Havana, Cuba", "Casablanca, Morocco", "Nairobi, Kenya",
    "Lagos, Nigeria", "Cairo, Egypt", "Jerusalem, Israel", "Mecca, Saudi Arabia", "Tehran, Iran",
    "Baghdad, Iraq", "Kyoto, Japan", "Hong Kong, China", "Shanghai, China", "Delhi, India",
    "San Francisco, USA", "Los Angeles, USA", "Chicago, USA", "Miami, USA", "Boston, USA",
    "Washington D.C., USA", "Seattle, USA", "Denver, USA", "Dallas, USA", "Atlanta, USA",
    "Hawaii, USA", "Alaska, USA", "Greenland", "Iceland", "Maldives",
    "Santorini, Greece", "Bali, Indonesia", "Bora Bora, French Polynesia", "Dubai, UAE", "Abu Dhabi, UAE"
]
    r=random.choice(c)
    print(r)
    return()
def place():
    n=int(input("Enter how many you want :"))
    a=1
    while(a<=n):
        placex()
        a+=1
    print("Thats all! I have provided you with ", n," places")  

def area(x):
    if "circle" in x:
        r=int(input("Enter the radius :"))
        a=math.pi*(r**2)
        print("Area of the circle with radius ",r,"=",round(a,4) )
    elif "triangle" in x:
        b=int(input("Enter the base :"))
        h=int(input("Enter the height :"))
        a=(1/2)*b*h
        print("Area of the triangle with base and height ",b,h,"respectively =",round(a,4) )
    elif "square" in x:
        b=int(input("Enter the side :"))
        a=b**2
        print("Area of the square with sides ",b,"=",round(a,4) )
    elif "rectangle" in x:
        b=int(input("Enter the width :"))
        l=int(input("Enter the length :"))
        a=l*b
        print("Area of the rectangle with width and length ",b,h,"respectively =",round(a,4) )
    elif "rhombus" in x or "parellogram" in x:
        b=int(input("Enter the base :"))
        h=int(input("Enter the height :"))
        a=b*h
        if "rombus" in x:
            print("Area of the rhombus with base and height ",b,h,"respectively =",round(a,4) )
        else:
            print("Area of the parellogram with base and height ",b,h,"respectively =",round(a,4) )
    elif "trapezium" in x:
        b1=int(input("Enter the base :"))
        b2=int(input("Enter the base :"))
        h=int(input("Enter the height :"))
        a=((1/2)*(b1+b2))*h
        print("Area of the trapezium with parallel sides and height ",b1,b2,h,"respectively =",round(a,4) )
    elif "cube" in x:
        b=int(input("Enter the sides :"))
        a=6*(a**2)
        print("SurfaceArea of the cube with sides",b,"=",round(a,4) ) 
    elif "cuboid" in x:
        l=int(input("Enter the length :"))
        b=int(input("Enter the base :"))
        h=int(input("Enter the height :"))
        a=2*((l*b)+(b*h)+(l*h))
        print("SurfaceArea of the cuboid with length,base and height ",l,b,h,"respectively =",round(a,4) )
    elif "sphere" in x:
        r=int(input("Enter the radius :"))
        a=4*math.pi*(r**2)
        print("SurfaceArea of the sphere with radius",r,"=",round(a,4) )
    elif "hemisphere" in x:
        r=int(input("Enter the radius :"))
        a=3*math.pi*(r**2)
        print("SurfaceArea of the hemisphere with radius",r,"=",round(a,4) )
    elif "cylender" in x:
        r=int(input("Enter the radius :"))
        h=int(input("Enter the height :"))
        a=2*math.pi*r*(r+h)
        print("SurfaceArea of the cylender with radius and height",r,h,"=",round(a,4) )
    elif "cone" in x:
        r=int(input("Enter the radius :"))
        h=int(input("Enter the height :"))
        a=math.pi*r*(r+h)
        print("SurfaceArea of the cone with radius and height",r,h,"=",round(a,4) )
    
    else:
        print("Sorry I cannot calculate the area of the given figure. Try again!!!  :(")

def perimeter(x):
    if "circle" in x:
        r=int(input("Enter the radius :"))
        a=2*math.pi*r
        print("Circumference of the circle with radius ",r,"=",round(a,4) )
    elif "triangle" in x:
        s1=int(input("Enter the side1 :"))
        s2=int(input("Enter the side2 :"))
        s3=int(input("Enter the side3 :"))
        a=s1+s2+s3
        print("Perimeter of the triangle with sides ",s1,s2,s3,"respectively =",round(a,4) )
    elif "square" in x:
        b=int(input("Enter the side :"))
        a=4*b
        print("Area of the square with sides ",b,"=",round(a,4) )
    elif "rectangle" in x:
        b=int(input("Enter the width :"))
        l=int(input("Enter the length :"))
        a=2*(l+b)
        print("Perimeter of the rectangle with width and length ",b,l,"respectively =",round(a,4) )
    else:
        print("Sorry I cannot calculate the perimeter of the given figure. Try again!!!  :(")

def volume(x):
    if "cube" in x:
        b=int(input("Enter the sides :"))
        a=(a**3)
        print("Volume of the cube with sides",b,"=",round(a,4) ) 
    elif "cuboid" in x:
        l=int(input("Enter the length :"))
        b=int(input("Enter the base :"))
        h=int(input("Enter the height :"))
        a=l*b*h
        print("Volume of the cuboid with length,base and height ",l,b,h,"respectively =",round(a,4) )
    elif "sphere" in x:
        r=int(input("Enter the radius :"))
        a=(4/3)*math.pi*(r**3)
        print("Volume of the sphere with radius",r,"=",round(a,4) )
    elif "hemisphere" in x:
        r=int(input("Enter the radius :"))
        a=(2/3)*math.pi*(r**3)
        print("Volume of the hemisphere with radius",r,"=",round(a,4) )
    elif "cylender" in x:
        r=int(input("Enter the radius :"))
        h=int(input("Enter the height :"))
        a=h*math.pi*r
        print("Volume of the cylender with radius and height",r,h,"=",round(a,4) )
    elif "cone" in x:
        r=int(input("Enter the radius :"))
        h=int(input("Enter the height :"))
        a=(1/3)*math.pi*h*(r**2)
        print("Volume of the cone with radius and height",r,h,"=",round(a,4) )
    
    else:
        print("Sorry I cannot calculate the volume of the given figure. Try again!!!  :(")

def jokex():
    c=[
    "A guy walks into a bar and says 'Ouch.' It was an iron bar.",
    "I'm reading a book on anti-gravity. It's impossible to put down!",
    "I haven't slept for ten days, because that would be too long.",
    "My wife asked me to go get 6 cans of Sprite from the grocery store. I realized when I got home that I had picked 7 up.",
    "I was wondering why the frisbee kept getting bigger. Then it hit me.",
    "The rotation of earth really makes my day.",
    "I used to play piano by ear, but now I use my hands.",
    "I'm worried for the calendar. Its days are numbered.",
    "I'm friends with all electricians. We just have good chemistry.",
    "A skeleton walks into a bar and orders a beer and a mop.",
    "To the person who stole my copy of Microsoft Office, I will find you. You have my Word!",
    "I want to die peacefully in my sleep, like my grandfather. Not screaming in terror like the passengers in his car.",
    "I told my boss that three companies were after me and I needed a raise. He asked which ones. I said the gas, electric, and water companies.",
    "Why can't a bike stand up by itself? It's two-tired.",
    "I told my girlfriend she was drawing her eyebrows too high. She looked surprised."
]
    r=random.choice(c)
    print(r)
    return()  
def jokes():
    while(True):
        jokex()
        c=input("To stop enter 's'")
        if "s" in c.lower():
            break
        else:
            continue   

def insqx():
    c=["The only way to do great work is to love what you do. – Steve Jobs",
    "Believe you can and you're halfway there. – Theodore Roosevelt",
    "It does not matter how slowly you go as long as you do not stop. – Confucius",
    "The future belongs to those who believe in the beauty of their dreams. – Eleanor Roosevelt",
    "Success is not final, failure is not fatal: it is the courage to continue that counts. – Winston Churchill",
    "Hardships often prepare ordinary people for an extraordinary destiny. – C.S. Lewis",
    "The only limit to our realization of tomorrow will be our doubts of today. – Franklin D. Roosevelt",
    "Do what you can, with what you have, where you are. – Theodore Roosevelt",
    "It always seems impossible until it's done. – Nelson Mandela",
    "The best way to predict the future is to create it. – Peter Drucker",
    "Don't watch the clock; do what it does. Keep going. – Sam Levenson",
    "Everything you've ever wanted is on the other side of fear. – George Addair",
    "The secret of getting ahead is getting started. – Mark Twain",
    "Your time is limited, so don't waste it living someone else's life. – Steve Jobs",
    "What you get by achieving your goals is not as important as what you become by achieving your goals. – Zig Ziglar"
]
    r=random.choice(c)
    print(r)
    return()  
def insq():
    while(True):
        insqx()
        c=input("To stop enter 's'")
        if "s" in c.lower():
            break
        else:
            continue   

def reply():
    a=["I can tell date,time,weekday,day of year",
       "I can solve small arethematic operation "
       " find sqroot,cuberoot,power of a number,area perimeter and volume of simple 2D and 3D figures",
       "I can also roll dice,toss coin, name animals,places, and people",
       "I can also play rock paper scissors ans tell jocks and motivational quotes"
       ]
    print(a)


def cb_response(user_choice):
    user_choice=user_choice.lower()
    if"hello" in user_choice or "hi" in user_choice or "hii" in user_choice:
        return"Hello! How can I help you? :)"
    elif"how are you" in user_choice:
        return"I am doing very well. Thank you for asking. :)"
    elif"who are you" in user_choice:
        return"I am a artificial friend developed by you using python programming language.If you want to know more about me you can ask for 'what can I do'"
    elif"bye" in user_choice:
        return"Goodbuy! Have a nice day ! See you next time ! :)"
    elif"date" in user_choice:
        return(date())
    elif"thank you" in user_choice or "thanks" in user_choice:
        return"You're most Welcome!!! The pleasure was all mine! :)"
    elif"time" in user_choice:
        return(time())
    elif"week day" in user_choice or "day of the week" in user_choice or "day" in user_choice:
        return(weekday())
    elif"day of year" in user_choice:
        return(day_of_year())
    elif"add" in user_choice or "subtract" in user_choice or "multiply" in user_choice or "divide" in user_choice:
        return(arethematic_op(user_choice))
    elif"cuberoot" in user_choice  or "squareroot" in user_choice  or "exponent" in user_choice  or "power of" in user_choice :
        return(maths(user_choice))
    elif"log with base 10" in user_choice or "log without base 10" in user_choice:
        return(log(user_choice))
    elif"roll the dice" in user_choice or "roll dice" in user_choice:
        return(dice())
    elif"toss the coin" in user_choice or "toss coin" in user_choice:
        return(coin())
    elif"rock paper scissors" in user_choice:
        return(rps())
    elif"pick a number from" in user_choice or "pick a number between" in user_choice:
        return(pick_a_num())
    elif"name some animals" in user_choice:
        return(animals())
    elif"great!" in user_choice or "well done!" in user_choice:
        return"Thank you for your appreciation! It means a lot :)"
    elif"name some colours" in user_choice:
        return(color())
    elif"name some famous individuals" in user_choice or "name some well known individuals" in user_choice or "name some well known peoples" in user_choice or "some famous people" in user_choice:
        return(people())
    elif"name some places" in user_choice:
        return(place())
    elif"area" in user_choice or "surface area" in user_choice:
        return(area(user_choice))
    elif"perimeter" in user_choice or "circumference" in user_choice:
        return(perimeter(user_choice))
    elif"volume" in user_choice:
        return(volume(user_choice))
    elif"jokes" in user_choice:
        return(jokes())
    elif"motivational" in user_choice or "inspritional" in user_choice:
        return(insq())
    elif"what can you do" in user_choice:
        return(reply())
    else:
        return"Sorry!!! I didn't get it. Try again! :|"


print("Welcome!!!") 
print("Chatbot : Hello type something(type 'bye' to exit)")
while(True):
    user = input("You : ")
    response = cb_response(user)
    print("Chatbot : ",response)
    if "bye" in user.lower():
        break  
