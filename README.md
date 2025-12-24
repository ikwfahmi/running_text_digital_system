# Running Text Digital System (VHDL)

Sistem teks berjalan (Running Text) yang diimplementasikan menggunakan bahasa pemrograman VHDL untuk desain sistem digital. Proyek ini mensimulasikan bagaimana data karakter digeser secara sekuensial untuk menciptakan efek teks bergerak pada display.

## 📌 Deskripsi Proyek
Proyek ini merupakan implementasi dari konsep dasar sistem digital yang meliputi:
* **Clock Division:** Menurunkan frekuensi clock tinggi ke frekuensi rendah agar teks bergerak dengan kecepatan yang sesuai.
* **Finite State Machine (FSM):** Mengatur alur logika penampilan karakter.
* **Shift Register Logic:** Logika pergeseran bit untuk menggerakkan data dari satu kolom ke kolom berikutnya.

## 📁 Struktur File
* `src/`: Berisi file sumber VHDL (.vhd).
* `sim/`: File testbench untuk keperluan simulasi software.
* `assets/`: Gambar atau diagram skema sistem (jika ada).

## 🛠️ Alat dan Bahan
* **Bahasa:** VHDL
* **Software:** Quartus Prime / ModelSim / Vivado / GHDL.
* **Hardware (Opsional):** FPGA Board (Altera Cyclone, Xilinx Artix, dll).

## 🚀 Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone [https://github.com/ikwfahmi/running_text_digital_system.git](https://github.com/ikwfahmi/running_text_digital_system.git)
