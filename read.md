``` markdown
# Verilənlərin Analizi Fənni Üzrə 5 CSV Faylının Analizi

Bu layihə **VS Code** və **Jupyter Notebook** mühitində 5 fərqli CSV faylının analiz edilməsi və hesabatın hazırlanması üçün nəzərdə tutulmuşdur.

> 💻 **Sistem Məlumatı:** Bu analiz Arch Linux bazalı **CachyOS** distributivi üzərində hazırlanmış və test edilmişdir.

---

## 🚀 Analizin Nəticələrinə Baxmaq Üçün Təlimat

Analizi öz lokal mühitinizdə rəvan işlətmək üçün aşağıdakı addımları ardıcıllıqla icra edin.

### Addım 1: Layihəni Açın
1. Göndərilmiş qovluğu ZIP arxivindən çıxarın.
2. ZIP-dən çıxarılmış qovluğu **VS Code** redaktoru vasitəsilə açın.

### Addım 2: Köhnə Virtual Mühiti Silin
* VS Code-da sol paneldə yerləşən fayl strukturuna gəlin və orada mövcud olan köhnə `venv` qovluğunu tamamilə **silin**.

### Addım 3: Lazımi VS Code Genişlənmələrini (Extensions) Yükləyin
Analizin düzgün vizuallaşdırılması üçün aşağıdakı genişlənmələrin quraşdırıldığından əmin olun:

* **Python & Mühit:** `Python`, `Pylance`, `Python Debugger`, `Python Environments`
* **Jupyter Dəstəyi:** `Jupyter`, `Jupyter Cell Tags`, `Jupyter Keymap`, `Jupyter Slide Show`, `Jupyter Notebook Renderers`
* **Terminal:** `PowerShell`

### Addım 4: Virtual Mühitin Yaradılması və Aktivləşdirilməsi
VS Code daxilində terminalı açın və növbə ilə aşağıdakı əmrləri icra edin:

1. **Yeni virtual mühit yaradın:**
   ```bash
   python -m venv venv

```

2. **PowerShell icazə siyasətini tənzimləyin** *(Skriptin işə düşməsi üçün)*:
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

```


3. **Virtual mühiti aktivləşdirin:**
```powershell
.\venv\Scripts\Activate.ps1

```



### Addım 5: Kitabxanaların Quraşdırılması

Analiz üçün lazımdır olan bütün asılılıqları (dependencies) yükləmək üçün terminalda bu əmri işə salın:

```bash
pip install -r requirements.txt

```

---

## 📊 Notebook-ların İşə Salınması

### Addım 6: Faylı Seçin və Kernel Təyin Edin

1. Qovluqdakı `analiz1.ipynb`, `analiz2.ipynb`, ..., `analiz5.ipynb` və ya `hesabat.ipynb` fayllarından istədiyiniz birini açın.
2. Seçdiyiniz faylın sağ üst küncündə yerləşən **"Select Kernel"** yazısına klikləyin.
3. Açılan siyahıdan az öncə yaratdığınız `venv` mühitini seçin.

> 💡 **Qeyd:** Əgər kodları çalışdıran zaman VS Code sizə yeni Python versiyası və ya əlavə paket yükləməyi tövsiyə edərsə, bunu təsdiqləyin.

### Addım 7: Kodları Çalışdırın (Mühüm Tövsiyə)

* Kodları işə salmazdan öncə, notebook-un yuxarı panelində yerləşən **"Clear All Outputs"** düyməsinə klikləyin. Bu, əvvəlki icra növündən qalan nəticələri təmizləyəcək və bütün prosesi sıfırdan, özünüz müşahidə edərək izləməyinizə imkan verəcək.
* Daha sonra kodları sətirbəsətir (tək-tək) və ya yuxarıdakı **"Run All"** əmri vasitəsilə birdəfəyə tam şəkildə çalışdıra bilərsiniz.

---

🙌 **Diqqətiniz üçün təşəkkürlər!**

```
```
