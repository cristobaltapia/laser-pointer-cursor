# Laser pointer cursor theme

This is a simple x-cursor theme that emulates a laser pointer.
Nothing fancy.
However, it is very useful in the times of online presentations.

And it looks like this:

![image description](preview.png)

## Installation

For local user installation, run the following command:

```sh
./install.sh
```

For system-wide installation, use the following command:

```sh
sudo ./install.sh
```

## Use case

I use [Sway](https://swaywm.org) as my window manager, where it is possible to define the cursor theme for a specific input device.
For example, I own a Logitech Spotlight device, which can be moved to its own _seat_, so that the laser pointer theme is only associated with this device.
In the sway configuration this can be achieved as follows:

```
seat seat_spotlight {
    attach 1133:50494:Logitech_USB_Receiver_Mouse
    hide_cursor 1000
    xcursor_theme "laser-pointer-cursors"
}
```

## F.A.Q.

* How did you do this?

    I didn't know anything about creating custom cursor themes, so I just copied most of what is in [this](https://github.com/vinceliuice/McMojave-cursors) repo.
    Then I did my own cursor with Inkscape.
