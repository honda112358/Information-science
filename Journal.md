#This is the journal for computer science

1. What did we do?
2. What did you learn?
1. What question do I have?

Answer
1. We made an argorithm for Mr. Ruben to make his breakfast by using two kinds of jam, bread and two knives.
2. I learned how much we are depending on the shared knowledge previously. Also, I learned that we have to use a unversal language which everyone can understand precisely.
3. How much information do I have to put into the computer? What kind of system does it have?



1, We played with degital dices. It was very hard to guess the correct number. It was even doubtful if we ordered correctly.

def setup():
    size(600, 600)
    
def draw():
    x=0
        
def mouseClicked():
    background(255)
    stroke(0)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)

    
    
    n=random(0,6)
    print(n)
    if 0<=n<1:
        circle(300,300,50)
    if 1<=n<2:
        circle(200,200,50)
        circle(400,400,50)
    if 2<=n<3:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
    if 3<=n<4:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
    if 4<=n<5:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
    if 5<=n<6:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
------------------------------------------------------------------------------------------------------------------------------
It was confusing for me to recognize what kind of variables or orders I should use since I hardky have knowledge about it. However, I'm getting how it works litttle by little. 
------------------------------------------------------------------------------------------------------------------------------

#These variables are to count the rools of the dice

ones=0
twos=0
threes=0
fours=0
fives=0
sixes=0

def setup():
    size(600, 600)
    
    
def draw():
    x=0
    barGraph()
    mouseClicked()
    barGraph()
    
def barGraph():
    global ones
    fill(0)
    textSize(20)
    for x in range (6):
        text(x+1, (90+90*x), 580)
        
        rect(90,550-ones,20,ones)
        rect(180,550-twos,20,twos)
        rect(270, 550-threes, 20, threes)
        rect(360,550-fours, 20, fours)
        rect(450, 550-fives, 20, fives)
        rect(540, 550-sixes,20,sixes)
        
def mouseClicked():
    global ones, twos, threes, fours, fives, sixes
    background(255)
    stroke(0)
    fill(255)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)

    
    
    n=random(0,6)
    print(n)
    if 0<=n<1:
        circle(300,300,50)
        ones=ones+1
        print("Number of times one has been rolled: ", ones)
    if 1<=n<2:
        circle(200,200,50)
        circle(400,400,50)
        twos=twos+1
        print("Number of times two has been rolled: ", twos)
    if 2<=n<3:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
        threes=threes+1
        print("Number of times three has been rolled: ", threes)
    if 3<=n<4:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        fours=fours+1
        print("Number of times four has been rolled: ", fours)
    if 4<=n<5:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
        fives=fives+1
        print("Number of times one has been rolled: ", fives)
    if 5<=n<6:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
        sixes=sixes+1
        print("Number of times six has been rolled: ", sixes)

------------------------------------------------------------------------------------------------------------------------------
white = 255
offset=50

def setup():
    size(500,500)
    background(255)
    
def draw():
    stroke(0)
    y=50
    for row in range(9):
         line(0,y,500,y)
         y=y+50
        
    fill(0)
    stroke(255)
    
    y=0
    for row in range(5):
        x=0
        for s in range(5):
            square(x,y, 50)
            x=x+100
        y=y+100
 
    #this are the odd rows
    y=50
    global offset
    for row in range(5):
        x=0 + offset
        for s in range(5):
            square(x,y, 50)
            x=x+100
        y=y+100
        
def mouseClicked():
    global offset
    offset=offset+1
    
------------------------------------------------------------------------------------------------------------------------------
