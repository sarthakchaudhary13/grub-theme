# My grub-theme

<img src = "https://preview.redd.it/roh9dg2s2m851.jpg?width=960&crop=smart&auto=webp&s=cba2a4896da57f0935d234fb1c7bb4a4d706762b">

# Installation
- Clone this repo  
`$git clone https://github.com/sarthakchaudhary13/grub-theme.git`

- Copy the theme to the bootloader themes directory (required root access)  
`sudo cp -a /path/to/cloned/repo /boot/grub/themes/grub-theme`

- Setting the theme (I am using vim here, you can use your preferred editor)
  - open default/grub  
   `sudo vim /etc/default/grub`
  - Find **GRUB_THEME=** if it's commented uncomment it and put the below code in it's place  
  `GRUB_THEME="/boot/grub/themes/grub-theme/theme.txt"`
  - Save and exit the editor
  
- Generate grub.cfg  
 `sudo grub-mkconfig -o /boot/grub/grub.cfg`
 
 - reboot  
 `reboot`
 
 - If you face any errors feel free to ask me by opening an issue
