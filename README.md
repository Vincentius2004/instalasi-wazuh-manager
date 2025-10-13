# instalasi-wazuh-manager

## Langkah 1 : pada ubuntu yang sudah di install lakukan update dan upgrade (Vincentius2004/instalasi-Ubuntu-Live-server-22.04)

![Teks alternatif untuk gambar](pict/wazuhman-tests%20%5BRunning%5D%20-%20Oracle%20VirtualBox%2010_12_2025%207_00_24%20PM.png)

## Langkah 2 : Jalankan perintah berikut untuk menambahkan repository dan GPG key dari Wazuh
    curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo gpg --dearmor -o /usr/share/keyrings/wazuh.gpg
    echo "deb [signed-by=/usr/share/keyrings/wazuh.gpg] https://packages.wazuh.com/4.x/apt/ stable main" | \
    sudo tee /etc/apt/sources.list.d/wazuh.list
![Teks alternatif untuk gambar](pict/wazuhman-tests%20%5BRunning%5D%20-%20Oracle%20VirtualBox%2010_12_2025%207_19_01%20PM.png)

## Langkah 3 : install wazuh managernya dengan cara 
    sudo apt install wazuh-manager -y
![Teks alternatif untuk gambar](pict/wazuhman-tests%20%5BRunning%5D%20-%20Oracle%20VirtualBox%2010_12_2025%207_20_49%20PM.png)

## Langkah 4 : setelah wazuh-manager terinstall kalian bisa menggunakan wazuh 
    sudo systemctl daemon-reload
    sudo systemctl enable wazuh-manager (mengaktivkan wazuh-manager)
    sudo systemctl start wazuh-manager (menjalankan aktivitas wazuh-manager)
    sudo systemctl stop wazuh-manager (melakukan stop aktivitas wazuh-manager)
![Teks alternatif untuk gambar](pict/wazuhman-tests%20%5BRunning%5D%20-%20Oracle%20VirtualBox%2010_12_2025%207_30_23%20PM.png)

## Untuk wazuh manager saat sudah aktif
![Teks alternatif untuk gambar](pict/wazuhman-tests%20%5BRunning%5D%20-%20Oracle%20VirtualBox%2010_12_2025%207_30_32%20PM.png)

## Untuk wazuh manager saat sudah inactive
![Teks alternatif untuk gambar](pict/wazuhman-tests%20%5BRunning%5D%20-%20Oracle%20VirtualBox%2010_12_2025%207_38_36%20PM.png)


























