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


