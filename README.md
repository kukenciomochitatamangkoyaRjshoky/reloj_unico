vertical_position = 0


def setup():
    size(250,500)
    
def draw():

    global vertical_position
    
    background(map(second(), 0, 59, 0, 255))
    noStroke()
    fill(map(second(), 0, 59, 255, 0))
    
    ellipse (width / 2, vertical_position, 10, 10)
    

    
    if vertical_position > height:
        vertical_position = 0
        
    else:
        vertical_position = map(second(), 0, 59, 0, height)
