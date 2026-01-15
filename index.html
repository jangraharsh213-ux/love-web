import tkinter as tk
import random

# ---------------- NO BUTTON RUNS AWAY ----------------
def move_no(event):
    button_width = 80
    button_height = 40

    max_x = root.winfo_width() - button_width
    max_y = root.winfo_height() - button_height

    x = random.randint(20, max_x)
    y = random.randint(150, max_y)

    no_button.place(x=x, y=y)


# ---------------- FLOWER CLASS ----------------
class Flower:
    def __init__(self, canvas, width):
        self.canvas = canvas
        self.x = random.randint(20, width - 20)
        self.y = -20
        self.size = random.randint(12, 20)
        self.speed = random.randint(2, 6)
        self.color = random.choice(["#ff69b4", "#ffb6c1", "#ffc0cb", "#ff85a2"])

        self.petals = []
        for dx, dy in [(-1,0),(1,0),(0,-1),(0,1),(-1,-1),(1,1)]:
            petal = canvas.create_oval(
                self.x + dx*self.size,
                self.y + dy*self.size,
                self.x + dx*self.size + self.size,
                self.y + dy*self.size + self.size,
                fill=self.color,
                outline=""
            )
            self.petals.append(petal)

        self.center = canvas.create_oval(
            self.x + self.size//2,
            self.y + self.size//2,
            self.x + self.size,
            self.y + self.size,
            fill="yellow",
            outline=""
        )

    def fall(self):
        for item in self.petals + [self.center]:
            self.canvas.move(item, 0, self.speed)
        self.y += self.speed

# ---------------- YES CLICKED ----------------
def yes_clicked():
    label.config(text="I knew it 💖")
    yes_button.destroy()

    root.geometry("600x500")
    root.configure(bg="#ffc0cb")

    canvas = tk.Canvas(root, width=600, height=500, bg="#ffc0cb", highlightthickness=0)
    canvas.pack()

    flowers = []

    def animate():
        if random.random() < 0.3:
            flowers.append(Flower(canvas, 600))

        for flower in flowers[:]:
            flower.fall()
            if flower.y > 520:
                flowers.remove(flower)

        root.after(30, animate)

    animate()

# ---------------- WINDOW ----------------
root = tk.Tk()
root.title("💖 Question 💖")
root.geometry("500x400")
root.resizable(False, False)

label = tk.Label(
    root,
    text="Do u love me?",
    font=("Arial", 22, "bold"),
    bg="white"
)
label.pack(pady=40)

yes_button = tk.Button(
    root,
    text="Yes 💕",
    font=("Arial", 14),
    command=yes_clicked
)
yes_button.place(x=160, y=220)

no_button = tk.Button(
    root,
    text="No 😒",
    font=("Arial", 14)
)
no_button.place(x=280, y=220)
no_button.bind("<Enter>", move_no)

root.mainloop()
