<div style="text-align:center;">

# Fast Forward <br/>
## **Rovines Derlan Hutabarat**

</div>

1. **Buat Folder Baru**

2. **Inisialisasi git**
    ```bash
    git init
    ```
3. **Buat File Readme.MD Pada Folder Yang Telah Dibuat**
4. **Tambahkan Text Pada File Readme**
5. **Tambahkan Branch Parent Dan Child**
    ```bash
    git checkout -b ParentRovines
    git checkout -b ChildRovines
    ```
6. **Pindah Ke Branch Child**
    ```bash
    git checkout ChildRovines
    ```
7. **Push Perubahan Ke Local Staging Area**
    ```bash
    git add .
    git commit -m "commit 1"
    ```
8. **Cek Perbedaan File Di Parent branch dan Child Branch**
    ```bash
    git checkout ParentRovines
    git checkout ChildRovines
    ```
9. **Lakukan Merge Ketika Posisi branch ada di Parent branch**
    ```bash
    git merge ChildRovines
    ```
10. **Push Ke Repository Github**
    ```bash
    git push origin ParentRovines
    ```
