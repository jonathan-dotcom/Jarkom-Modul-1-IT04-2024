# Lapres Modul 1 Jarkom IT-04

## creds

1. Cari satu satu dari package, dan cari isi package paling lengkap. Lalu coba follow data package yang lengkap dengan coba case setiap datanya.
2. Dalam pencarian, coba filter package dengan display filter, untuk inputnya adalah FTP. Pemfilteran ini agar mempermudahkan kita dalam mencari informasi flag.
3. Dari banyaknya packageKita bisa tahu terdapat percobaan login, kita hanya perlu memeriksa setiap isinya
    
    ![https://lh7-us.googleusercontent.com/zYZPXWSRhC-dIXnpS4P8k4uGEVoUOC37-BY0syvE_Rf-mTXPuupQdLYuYJ1mHUROkgIvdzpWoLRSGzFv4j5uQOY97qLZzL7POdGzPkxs_0hS5iwqGnWo5XyJY6XkrEiXpr6kDN7hQaaCCLO9i_hJ_A](https://lh7-us.googleusercontent.com/zYZPXWSRhC-dIXnpS4P8k4uGEVoUOC37-BY0syvE_Rf-mTXPuupQdLYuYJ1mHUROkgIvdzpWoLRSGzFv4j5uQOY97qLZzL7POdGzPkxs_0hS5iwqGnWo5XyJY6XkrEiXpr6kDN7hQaaCCLO9i_hJ_A)
    
4. Dengan memilih yang terdapat Informasi Login Successful, isinya sebagai berikut
    
    ![https://lh7-us.googleusercontent.com/CanQZrFSHa7tgc6og40ng0gFT_064ItvLHMffT2ub6Xo90by9Hve0ayEVPIv7RejEHzGgnqVYIdazl6XGGN4qFj-LqZIe1WLG7fKpv3YhK7dc2GLIGhftwMKVH3isi8LOtslRUGfeuhcCAfMbSEWXg](https://lh7-us.googleusercontent.com/CanQZrFSHa7tgc6og40ng0gFT_064ItvLHMffT2ub6Xo90by9Hve0ayEVPIv7RejEHzGgnqVYIdazl6XGGN4qFj-LqZIe1WLG7fKpv3YhK7dc2GLIGhftwMKVH3isi8LOtslRUGfeuhcCAfMbSEWXg)
    
5. Maka kita bisa menginputkan case user dan passowrd yang terdapat log login successful tersebut.
6. Saat dicoba pada ncat maka hasilnya sebagai berikut
    
    ![https://lh7-us.googleusercontent.com/yCvq4CYvacmvgvFlVr7sgV07ie2D1Q8yPIuor5sHvgaCwdEFZLDELkLFXHvUrUkh2beBR_g1QrSedoUux6rrubdhAkHcCjOfWpqdMkAt9ybgX8LEqgJSU1W61wdyLW2pTx668djUhZtxsNgAcnuq5g](https://lh7-us.googleusercontent.com/yCvq4CYvacmvgvFlVr7sgV07ie2D1Q8yPIuor5sHvgaCwdEFZLDELkLFXHvUrUkh2beBR_g1QrSedoUux6rrubdhAkHcCjOfWpqdMkAt9ybgX8LEqgJSU1W61wdyLW2pTx668djUhZtxsNgAcnuq5g)
    

## **malwleowleo**

1. Dalam informasi package yang didapatkan dari soal **CREDS,** kita mendapatkan informasi bahwa terdapat aktivitas STOR malicious_malware.c
    
    ![https://lh7-us.googleusercontent.com/LVEmrBlumgz0142ec3Jvdz_wpp0RcG4PK49kqGoyHrr_d5Nl5AaNn3VBJXpgKWFWFKHnoDDUlAvIpHd47zESFwjrMfF09WnuI19-92BH64v_rM69-G7xNPyS3lyZaO19s1IQRiH72qMFBpqGraT9_Q](https://lh7-us.googleusercontent.com/LVEmrBlumgz0142ec3Jvdz_wpp0RcG4PK49kqGoyHrr_d5Nl5AaNn3VBJXpgKWFWFKHnoDDUlAvIpHd47zESFwjrMfF09WnuI19-92BH64v_rM69-G7xNPyS3lyZaO19s1IQRiH72qMFBpqGraT9_Q)
    
    ![https://lh7-us.googleusercontent.com/hYnw4LcVK8TxUDDqv6b1H0dwhRblOkLpcP15QyZoY_9B2kkEo-CcSIqTajWWzi_1212zOKK4eZ_9wNUG2pyp9Gmrxh55eCDdnG-ScTHeB2gHY4CVq7E62mrerk3Y_nfjOZxlHhdiQajruydfQJtXPQ](https://lh7-us.googleusercontent.com/hYnw4LcVK8TxUDDqv6b1H0dwhRblOkLpcP15QyZoY_9B2kkEo-CcSIqTajWWzi_1212zOKK4eZ_9wNUG2pyp9Gmrxh55eCDdnG-ScTHeB2gHY4CVq7E62mrerk3Y_nfjOZxlHhdiQajruydfQJtXPQ)
    

## **whoami**

1. Pertanyaan dari soal whoami adalah berikut
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled.png)
    
2. Melanjutkan dari yang malwleowleo ternyata setelah kita lihat, dalam file malicious_malware.c yang dikirim oleh attacker terdapat text yang memiliki ciri ciri Base64
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%201.png)
    
3. Kita copy lalu, kita decode
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%202.png)
    
    Hasilnya sudah terlihat, bahwa nama yang diperlukan untuk mendapatkan flag adalah Paul Atreides
    
4. Seperti yang tertera pada tangkapan layar, nama tersebut ternyata benar
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%203.png)
    

## **secret**

1. Pertanyaan dari soal secret adalah sebagai berikut
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%204.png)
    
2. Jadi karena pesan rahasia ada di file yang dikirim attacker, maka kita bisa lihat dengan export object FTP-DATA sehingga kita dapat melihat file-nya
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%205.png)
    
3. Karena file .c sudah kita periksa tadi dan hanya terdapat nama attacker yang ter-encode, jadi kita akan memeriksa file lain yang dikirimkan attacker yaitu mirza.jpg. untuk melihatnya kita save dulu file-nya.
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%206.png)
    
4. Berikut filenya mirza.jpg-nya
    
    ![mirza.jpg](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/mirza.jpg)
    
5. Sesuai dengan soal, “temukan pesan yg dikutip oleh attacker” maka jawabannya adalah MIO MIRZA
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%207.png)
    

## ATM or ATP or FTP ? 🤔

1. Pertanyaan adalah ini,
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%208.png)
    
2. Disitu sudah disebutkan attacker melakukan bruteforce login ftp, jadi disini kata kuncinya ftp.
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%209.png)
    
    lalu kita cari-cari sampai ketemu yang successful dengan disearch
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%2010.png)
    
3. Sudah terlihat bahwa password yang berhasil adalah m4y_th3_Kn!fe_ch1p_&_sh4tter
    
    ![Untitled](Lapres%20Modul%201%20Jarkom%20IT-04%20e2fcbcf1000843548a8e737926654d20/Untitled%2011.png)
    

## **How Many packets?**

1. Kita filter terlebih dahulu dengan display filter ftp lagi agar mempermudah apa yang perlu kita cari
    
    ![https://lh7-us.googleusercontent.com/hgXFWMuGbRqgQd06EtYdUxpkI5zpUQ7JGjVWfp66aVx6M2-qTtVhaMvHpFJ9GvELYOswK8J5HvaDY4WVnGW1176CRcRWPBUEvKwe82WU71ImkzKHv-q0U1-YkDNt2O1WqIde0QYkIcEVKCJ_uyl-3Q](https://lh7-us.googleusercontent.com/hgXFWMuGbRqgQd06EtYdUxpkI5zpUQ7JGjVWfp66aVx6M2-qTtVhaMvHpFJ9GvELYOswK8J5HvaDY4WVnGW1176CRcRWPBUEvKwe82WU71ImkzKHv-q0U1-YkDNt2O1WqIde0QYkIcEVKCJ_uyl-3Q)
    
2. Setelah kita sorting berdasarkan info, kita tahu ada banyak jumlah login yang terjadi. Maka kita select all pada respon login tersebut dan kita export specified packets agar number tereset dari 1 untuk packet yang terdapat informasi login
3. Disini saya beri nama file “login.pcap” agar berbeda, lalu kita bisa tahu bahwa urutan number sudah tereset
    
    ![https://lh7-us.googleusercontent.com/1zKZxfXZhFimv9UufaE8xQN4HktxBOiy6dmBmIX-gV4CPybaloGw4mNTtqF_Hscl_iTKQpScDuQbNbr6H0Kggd5Ftb7NR2C7J0I2OyaNJ_1PxV4zAMXNFJfOQaVj3ltxbeEvHPn7FmExpSNRV7MKIA](https://lh7-us.googleusercontent.com/1zKZxfXZhFimv9UufaE8xQN4HktxBOiy6dmBmIX-gV4CPybaloGw4mNTtqF_Hscl_iTKQpScDuQbNbr6H0Kggd5Ftb7NR2C7J0I2OyaNJ_1PxV4zAMXNFJfOQaVj3ltxbeEvHPn7FmExpSNRV7MKIA)
    
    ![https://lh7-us.googleusercontent.com/wTdc9IGIIocOKYj46WcfaXojP1rNfIvy_7FmYoNmzdVSPEUwyDKMGgRQNM2mkwVQE9btrFqbhBpJ3mNTxHJECDv9LkM4k0YM6_Bw5Q9UrnQ_hCwan7Y1YHtljS8dT6zn-g75zq6Ue9aDZ_aHLPUOmA](https://lh7-us.googleusercontent.com/wTdc9IGIIocOKYj46WcfaXojP1rNfIvy_7FmYoNmzdVSPEUwyDKMGgRQNM2mkwVQE9btrFqbhBpJ3mNTxHJECDv9LkM4k0YM6_Bw5Q9UrnQ_hCwan7Y1YHtljS8dT6zn-g75zq6Ue9aDZ_aHLPUOmA)
    
4. Disini kita bisa tahu ada 933 packets yang terdapat informasi usaha login, maka kita hanya perlu menambahkan 1 usaha login lagi, karena yang kita dapatkan adalah usaha login yang gagal! Maka logikanya kita perlu menambahkan usaha login yang berhasil
    
    ![https://lh7-us.googleusercontent.com/rSINFinYl7TOjKhFRnvQVJ0sQ20Ci8FrbK__r98rc5T5WT89uXj3wK0pCT7GocabzLmcLpdJMn5XX2_ZNsWcZXqA-XYZt_D7LFkQXHdDNH7pnp8hgrQazfcKwwoe9yJG7266WWknYBt-yA_eZJnHpA](https://lh7-us.googleusercontent.com/rSINFinYl7TOjKhFRnvQVJ0sQ20Ci8FrbK__r98rc5T5WT89uXj3wK0pCT7GocabzLmcLpdJMn5XX2_ZNsWcZXqA-XYZt_D7LFkQXHdDNH7pnp8hgrQazfcKwwoe9yJG7266WWknYBt-yA_eZJnHpA)
    

## **Trace Him**

1. Disini, kita sebenarnya sudah dapat informasi IP attackerdimana pada usaha login, terdapat destination dari ip attacker
    
    ![https://lh7-us.googleusercontent.com/yx716zfFW0N7fOLX47UpMhPPmYwCpICJCC98YZgCvwz5_Gkp66vtXrPlRnmnKXkYdGvQYFOHFHswNmkDl6DjmxCJfSZ6n-8dXjbLFatmhwOpO_M2FVNrFt37K0KrNLQ2YL8fKLS8zmbvcny7JJnI1A](https://lh7-us.googleusercontent.com/yx716zfFW0N7fOLX47UpMhPPmYwCpICJCC98YZgCvwz5_Gkp66vtXrPlRnmnKXkYdGvQYFOHFHswNmkDl6DjmxCJfSZ6n-8dXjbLFatmhwOpO_M2FVNrFt37K0KrNLQ2YL8fKLS8zmbvcny7JJnI1A)
    
2. Kita bisa memakai ip tersebut untuk mencari tahu apakah benar itu ip dari usaha login
    
    ![https://lh7-us.googleusercontent.com/agv433-YHjObt-ORmnMruEpssJ9Lcb5iFsf1GR-fDHUSmtYSEPttWcMn723xjOPZf2SQH0k2cpFf1HXGjeHmZXMbTMOBs-Eb4_3hku-SNs16i3X2bDIzD-h1gSW6_VSysqHkKXGq1uw2oxKEj68Uww](https://lh7-us.googleusercontent.com/agv433-YHjObt-ORmnMruEpssJ9Lcb5iFsf1GR-fDHUSmtYSEPttWcMn723xjOPZf2SQH0k2cpFf1HXGjeHmZXMbTMOBs-Eb4_3hku-SNs16i3X2bDIzD-h1gSW6_VSysqHkKXGq1uw2oxKEj68Uww)
    

## **Evidence**

1. Cari salah satu package yang memiliki informasi HTTP dan server seperti berikutAgar lebih mudah, dikarenakan usaha membobol termasuk usaha login, kita tambahkan contains login pada filter meskipun itu incorrecct, bisa http maupun tcp (disini memakai tcp)
    
    ![https://lh7-us.googleusercontent.com/IDK6tk0xqf1LBZwWTBlcmeCJg_XBLOUkdPwImfrakNuTTqkYCPDpOIv-vhv4YceG6J9ltEf7ZP36UAsrxRqrXxPp_u7YK6hCIE-Wlz0za3ADuJaa4F9PaGzen8upQOiKAWeFZrHGxmiaR36KrJCcnA](https://lh7-us.googleusercontent.com/IDK6tk0xqf1LBZwWTBlcmeCJg_XBLOUkdPwImfrakNuTTqkYCPDpOIv-vhv4YceG6J9ltEf7ZP36UAsrxRqrXxPp_u7YK6hCIE-Wlz0za3ADuJaa4F9PaGzen8upQOiKAWeFZrHGxmiaR36KrJCcnA)
    
2. Lalu kita bisa follow packet tersebut (disini dalam kondisi login successful)
    
    ![https://lh7-us.googleusercontent.com/zAFRrZz6v2r40eYV3Ep60ay-jon-z4M28WS9ol5P3UENP3nhxezEDwiEr3mRsOVKkLobOaV_VKoo67luGMb-JvZQ10vclWJUTPskXfVmhmkieS7a1yZf5-FJnI0WD-ZzaSR0u7T8WGwxXaXIhOVHXQ](https://lh7-us.googleusercontent.com/zAFRrZz6v2r40eYV3Ep60ay-jon-z4M28WS9ol5P3UENP3nhxezEDwiEr3mRsOVKkLobOaV_VKoo67luGMb-JvZQ10vclWJUTPskXfVmhmkieS7a1yZf5-FJnI0WD-ZzaSR0u7T8WGwxXaXIhOVHXQ)
    
3. Dari informasi tersebut, kita sudah mendapatkan semua yang dibutuhkan. Namun, agar yang kita dapat berupa informasi Login Successful, maka kita perlu menambahkan Login Successful pada display filter -> tcp contains “Login Successful” dengan hasil ncat sebagai berikut Dapat dilihat bahwa %40 merupakan representasi symbol @ dalam format url
    
    ![https://lh7-us.googleusercontent.com/PU2ooQMI1sc8DRP_6N1yajZYOie2U6G1Qw2XnsrFcyodTufvs1CkrsvW7hz897VgRWEM7Onry6NfSMy0Dqi_iZKu8Ucr_XbnCTNmYJ7GxEFsyfFkN21qyJnEcBoPett2xPRMJp-pac9F4SYci44LTA](https://lh7-us.googleusercontent.com/PU2ooQMI1sc8DRP_6N1yajZYOie2U6G1Qw2XnsrFcyodTufvs1CkrsvW7hz897VgRWEM7Onry6NfSMy0Dqi_iZKu8Ucr_XbnCTNmYJ7GxEFsyfFkN21qyJnEcBoPett2xPRMJp-pac9F4SYci44LTA)
    

## **FUZZ**

1. Kita coba filter http untuk memudah pencariandan kita coba pilih salah satu packet yang memiliki banyak informasi didalamnya, dapat diketahui pada ip destination, merupakan ip flag dan saat kita buka lebih akan ada informasi tambahan
    
    ![https://lh7-us.googleusercontent.com/GQ90TwwUNYJO7xHSk5EHYVG2Y1XYciofg8riEkFDKtLYLq-Vrx-fW7pOWHNLKOfBpLCeQ-Xn-IOnkArF3nBAlpmQ9RvZdjpuMJI2iNHJtPKp82KH_xHdYrgF_877n1xFQg1gEIRGQbfY3zhHSv5Jcw](https://lh7-us.googleusercontent.com/GQ90TwwUNYJO7xHSk5EHYVG2Y1XYciofg8riEkFDKtLYLq-Vrx-fW7pOWHNLKOfBpLCeQ-Xn-IOnkArF3nBAlpmQ9RvZdjpuMJI2iNHJtPKp82KH_xHdYrgF_877n1xFQg1gEIRGQbfY3zhHSv5Jcw)
    
2. Pada informasi tambahan, terdapat src port 80 yang bisa kita pakai
    
    ![https://lh7-us.googleusercontent.com/-oV4BoogNcG15aqh6OPsIB4QSM6iema_d3fUCDKsw0TI_qvPwWFOpOPOaVt3k6x242TqXrAswsxsEtk3gGhGBpQMfLLYUxxvO0IUVcbNYVSrzAoIAHKV2OdLg5-M4yD4jPDulKeqVNWu1-YzDMHV5g](https://lh7-us.googleusercontent.com/-oV4BoogNcG15aqh6OPsIB4QSM6iema_d3fUCDKsw0TI_qvPwWFOpOPOaVt3k6x242TqXrAswsxsEtk3gGhGBpQMfLLYUxxvO0IUVcbNYVSrzAoIAHKV2OdLg5-M4yD4jPDulKeqVNWu1-YzDMHV5g)
    
3. Dan pada isi packet, terdapat banyak informasi yang bisa digunakan
    
    ![https://lh7-us.googleusercontent.com/A4E8sgd0RmVbgT3_JgtXqawQFypOvqOGpWdOckGzqNoczPGj27bhYVYE8q_uzemiMgtN_eDAFIHBO1bS4yB-Da3aJ_CzwXyEtvNCiDMnohvaCkJRYdj36X14dO-yf-PVSBKn9pS0MDy36akWSSoY8A](https://lh7-us.googleusercontent.com/A4E8sgd0RmVbgT3_JgtXqawQFypOvqOGpWdOckGzqNoczPGj27bhYVYE8q_uzemiMgtN_eDAFIHBO1bS4yB-Da3aJ_CzwXyEtvNCiDMnohvaCkJRYdj36X14dO-yf-PVSBKn9pS0MDy36akWSSoY8A)
    
    ![https://lh7-us.googleusercontent.com/QEHgqvYi4l5LJMt46e6BHWCw2QbeN1b_DVN-28ZpynRMRd4DsBfOk0YMNnitc2501SGUjrtMalwL-pQpnv8GjKIw1I9IsPkbiGbPkOHmG_UJCYSFDq54t9N2esW6Em2_0sIWmBrsxJ2sriORLNjiXw](https://lh7-us.googleusercontent.com/QEHgqvYi4l5LJMt46e6BHWCw2QbeN1b_DVN-28ZpynRMRd4DsBfOk0YMNnitc2501SGUjrtMalwL-pQpnv8GjKIw1I9IsPkbiGbPkOHmG_UJCYSFDq54t9N2esW6Em2_0sIWmBrsxJ2sriORLNjiXw)
    
4. Dari semua informasi yang didapat, dapat kita coba masukkan sebagai berikut (Masih gagal)
    
    ![https://lh7-us.googleusercontent.com/eqKYcx74hrO2Q191RHrsPlShwcRxXmzpbRZ08OxFxktyiKVVb_fW4ApixDG1r-Lgu2EIlpQU4PPnAegqjtzdXx6MOYKR2YuuvurOU8MJand3FNNqnkdZM55-4JNBZgAhGAWHd4cYR2MKtEE5G6kFEg](https://lh7-us.googleusercontent.com/eqKYcx74hrO2Q191RHrsPlShwcRxXmzpbRZ08OxFxktyiKVVb_fW4ApixDG1r-Lgu2EIlpQU4PPnAegqjtzdXx6MOYKR2YuuvurOU8MJand3FNNqnkdZM55-4JNBZgAhGAWHd4cYR2MKtEE5G6kFEg)
    
    ![https://lh7-us.googleusercontent.com/R791ufqa0kUIxV2-fsO-w9uhEb-XtnyA6m1rzWp4QIY1pT1cnWbYHaCol8KrtyKplAXtl3dVNOD31_qNA4w6IxCWSE54KiNaEKSpIDOYOdYwUgrX14ZvNYxMGmp6lNvtwa_YLywstpONleU57ki1Jg](https://lh7-us.googleusercontent.com/R791ufqa0kUIxV2-fsO-w9uhEb-XtnyA6m1rzWp4QIY1pT1cnWbYHaCol8KrtyKplAXtl3dVNOD31_qNA4w6IxCWSE54KiNaEKSpIDOYOdYwUgrX14ZvNYxMGmp6lNvtwa_YLywstpONleU57ki1Jg)