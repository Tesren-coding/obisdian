**Pygame** is a Python library for making **2D games and interactive visual applications**.

It gives you tools for things like:

- opening a game window
- drawing shapes and images
- playing sounds
- detecting keyboard and mouse input
- moving objects around the screen
- handling collisions
- controlling frame rate
---
Installing Pygame
```bash
pip install pygame
```

Example of "game loop"
```python
# Example file showing a basic pygame "game loop"
import pygame

# pygame setup
pygame.init()
screen = pygame.display.set_mode((1280, 720))
clock = pygame.time.Clock()
running = True

while running:
    # poll for events
    # pygame.QUIT event means the user clicked X to close your window
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # fill the screen with a color to wipe away anything from last frame
    screen.fill("purple")

    # RENDER YOUR GAME HERE

    # flip() the display to put your work on screen
    pygame.display.flip()

    clock.tick(60)  # limits FPS to 60

pygame.quit()
```
opens the window, updates the screen, and handles events