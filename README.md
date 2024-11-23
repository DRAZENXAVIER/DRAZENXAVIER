import time
import os

def animate_hearts_and_flowers():
    frames = [
        """
         @@@   @@@
        @   @ @   @
         @   @   @
          @     @
           @   @
            @ @
             @
        """,
        """
           ,@@@,   ,@@@,
          ,@@@@@@,@@@@@@,
          ,@@@@@@@@@@@@@,
           ,@@@@@@@@@@@,
            ,@@@@@@@@@,
             ,@@@@@@@,
              ,@@@@@,
               ,@@@,
                ,@,
        """,
        """
            \ | /
         '-. @ @ .-'
         ---  *  ---
         .-' @ @ '-.
            / | \\
        """
    ]
    for _ in range(3):  # Loop through the animations a few times
        for frame in frames:
            os.system('cls' if os.name == 'nt' else 'clear')  # Clear screen
            print(frame)
            time.sleep(0.5)

def confess_to_crush():
    name = "Kristine"
    hobbies = ["playing chess", "being an amazing journalist"]
    admirer_message = f"""
    Dear {name},

    I just wanted to share something from my heart. 
    You're so pretty, and your personality is amazing! 
    I really admire you for so many things, like your love for {hobbies[0]} 
    and your incredible talent as {hobbies[1]}.

    Someday, I hope we can meet and maybe play a game of chess together. 
    For now, I’m not ready to reveal my identity, but I want you to know 
    that you have a secret admirer who thinks you're absolutely wonderful.

    With admiration,
    A Secret Admirer
    """
    return admirer_message


# Animate hearts and flowers
animate_hearts_and_flowers()

# Print the confession
print(confess_to_crush())



