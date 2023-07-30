Import tkinter as tk

From tkinter import messagebox

Import time

Def set_alarm():

    Alarm_time = entry.get()

    While True:

        Current_time = time.strftime(“%H:%M:%S”)

        If current_time == alarm_time:

            Messagebox.showinfo(“Alarm”, “Time to wake up!”)

            Break



Root = tk.Tk()

Root.title(“Alarm Clock”)

Root.geometry(“300x150”)



# Create a label and entry for setting the alarm time

Label = tk.Label(root, text=”Enter the alarm time (HH:MM:SS):”)

Label.pack()

Entry = tk.Entry(root)

Entry.pack()



# Create a button to set the alarm

Set_button = tk.Button(root, text=”Set Alarm”, command=set_alarm)

Set_button.pack()



# Start the main event loop

Root.mainloop()



