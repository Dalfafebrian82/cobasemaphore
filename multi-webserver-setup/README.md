# Otomatisasi Setup Multi Web Server
Proyek ini menggunakan Ansible untuk menginstal Apache di beberapa server sekaligus dan mengatur halaman index sederhana.

## Cara Pakai
1. Edit `inventory/hosts.ini` dengan IP server Anda.
2. Jalankan dengan:
   ```bash
   ansible-playbook -i inventory/hosts.ini playbooks/setup_web.yml
   ```
3. Atau jalankan via **Ansible Semaphore**:
   - Tambahkan repository ini ke Project Semaphore.
   - Buat Inventory sesuai `hosts.ini`.
   - Buat Template dengan path `playbooks/setup_web.yml`.
   - Jalankan template dan cek hasil di browser.
