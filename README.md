### 🇺🇸 English:

##  Description
This repository provides detailed instructions and scripts to reset the login password on Linux systems using the GRUB bootloader.

## 🔧 Usage

Follow the steps below to use GRUB and reset the root password of your Linux operating system.

### 🛠️ Steps

1. **Access GRUB**
   - Boot the computer and access the GRUB menu. If it doesn't appear, press a key like `Esc` or `Shift` during startup.

2. **Modify Boot Options**
   - Select the desired boot option (usually the first one) and press `e` to edit the boot options.

3. **Add `init=/bin/bash` to Boot Options**
   - Find the line starting with `linux` or `kernel` and add `init=/bin/bash` at the end of that line.

4. **Boot into Single User Mode**
   - Press `Ctrl + X` or `F10` to boot the system with the new options. This will start the system directly into a root shell without requiring a password.

5. **Change the Root Password**
   - Once in the root shell (`#`), use the `passwd` command to change the root password:
     ```
     passwd
     ```
     Follow the on-screen instructions to enter and confirm the new password.

6. **Reboot the System**
   - After changing the password, reboot the system using:
     ```
     reboot
     ```
     The system should start normally, allowing you to access it with the new root password.

---

###  🇮🇹 Italiano:

##  Descrizione
Questo repository fornisce istruzioni dettagliate e script per reimpostare la password di accesso su sistemi Linux utilizzando il bootloader GRUB.

## 🔧 Utilizzo

Segui i passaggi di seguito per utilizzare GRUB e reimpostare la password di root del tuo sistema operativo Linux.

### 🛠️ Passaggi

1. **Accedere a GRUB**
   - Avvia il computer e accedi al menu di GRUB. Se non compare, premi un tasto come `Esc` o `Shift` durante l'avvio.

2. **Modificare le Opzioni di Avvio**
   - Seleziona l'opzione di avvio desiderata (solitamente la prima) e premi `e` per modificare le opzioni di avvio.

3. **Aggiungere `init=/bin/bash` alle Opzioni di Avvio**
   - Trova la riga che inizia con `linux` o `kernel` e aggiungi `init=/bin/bash` alla fine di quella riga.

4. **Avviare il Sistema in Modalità Singolo Utente**
   - Premi `Ctrl + X` o `F10` per avviare il sistema con le nuove opzioni. Questo avvierà il sistema direttamente in una shell di root senza richiedere la password.

5. **Cambiare la Password di Root**
   - Una volta nella shell di root (`#`), utilizza il comando `passwd` per cambiare la password di root:
     ```
     passwd
     ```
     Segui le istruzioni a schermo per inserire e confermare la nuova password.

6. **Riavviare il Sistema**
   - Dopo aver cambiato la password, riavvia il sistema usando il comando:
     ```
     reboot
     ```
     Il sistema dovrebbe avviarsi normalmente, consentendoti di accedere con la nuova password di root.

