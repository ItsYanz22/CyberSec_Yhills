## 🛠️ How to Download and Install VirtualBox

1. **Visit the Official Website**  
   Go to [https://www.virtualbox.org](https://www.virtualbox.org)

2. **Choose the Installer**  
   Click on the **Downloads** section and pick the version suitable for your OS (Windows, macOS, or Linux).

3. **Run the Installer**  
   Launch the downloaded file and follow the installation wizard. Keep default settings unless you know what to change.

4. **Install the Extension Pack (Optional but Recommended)**  
   Download from the same page. In VirtualBox, go to File → Preferences → Extensions → Add, and install it.

5. **Launch VirtualBox**  
   After installation, open VirtualBox to ensure it's running properly. You’re ready to create/import VMs.

---

## 🐱‍💻 How to Download Kali Linux and Open it in VirtualBox

1. **Download Kali Linux VM Image**  
   Visit [https://www.kali.org/get-kali/#kali-virtual-machines](https://www.kali.org/get-kali/#kali-virtual-machines) and download the **VirtualBox (OVA)** version.

2. **Verify the Download (Optional)**  
   Check the SHA256 hash provided on the website to verify file integrity (optional but recommended).

3. **Import into VirtualBox**  
   Open VirtualBox → File → Import Appliance → Select the downloaded `.ova` file → Click "Next" → "Import".

4. **Adjust System Settings (Optional)**  
   You can modify RAM, CPU, or network settings before starting the VM.

5. **Start the Kali Linux VM**  
   Click on the imported VM and press "Start". Kali Linux will boot up and be ready to use.

---

## 🔍 What to Do After Second Boot of Kali Linux

1. **Update Kali Linux**  
   Open the terminal and run:  
   ```bash
   sudo apt update && sudo apt upgrade -y
