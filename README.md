## Generic Raspberry Pi

### pre-boot patches
ansible-playbook retropie_pre_boot.yml

### post-boot seeding
ansible-playbook retropie_seeding.yml

## Retroflag GPI Case 1 (with pi zero 2)

### fetch latest image
ansible-playbook retroflag_gpi_fetch_image.yml 

### pre-boot patches
ansible-playbook retroflag_gpi_pre_boot.yml

### post-boot seeding
ansible-playbook retroflag_gpi_seeding.yml

## Retroflag GPI Case 2

### flash

gzip -dc data/os_images/retropie-buster-4.7.20-rpi2_3.img.gz | sudo dd of=/dev/mmcblk0 bs=64M
or
gzip -dc data/os_images/retropie-buster-4.7.1-rpi4_400.img.gz | sudo dd of=/dev/mmcblk0 bs=64M

### fetch latest image
ansible-playbook retroflag_gpi2_fetch_image.yml

### pre-boot patches
ansible-playbook retroflag_gpi2_pre_boot.yml

### post-boot seeding
ansible-playbook retroflag_gpi2_seeding.yml

## Retroflag NES Pi 4 case

### fetch latest image
ansible-playbook retroflag_nespi4_fetch_image.yml

### pre-boot patches
ansible-playbook retroflag_nespi4_pre_boot.yml

### post-boot seeding
ansible-playbook retroflag_nespi4_seeding.yml