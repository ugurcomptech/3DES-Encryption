# 3DES (Triple Data Encryption Standard) Şeması

3DES, orijinal Data Encryption Standard (DES) algoritmasının güvenliğini artırmak için geliştirilmiş bir şifreleme yöntemidir. Temel olarak, 3DES aynı DES algoritmasını üç farklı anahtarla üç kez uygulayarak veriyi şifreler.

## Algoritma Şeması

![image](https://github.com/ugurcomptech/3DES-Encryption/assets/133202238/1c92718e-f91a-453e-9728-7c6cb7c7afc7)



## Açıklama

- İlk adımda, veri (64 bit) ve ilk anahtar (64 bit) kullanılarak DES şifrelemesi yapılır.
- Elde edilen şifreli veri, ikinci anahtar (64 bit) kullanılarak DES şifre çözme işlemine tabi tutulur.
- Çözülen veri, üçüncü anahtar (64 bit) kullanılarak DES şifrelemesi yapılır.
- Elde edilen şifreli veri, yine ikinci anahtar (64 bit) kullanılarak DES şifre çözme işlemine tabi tutulur.
- Bu aşamada elde edilen çözülmüş veri, ilk anahtar (64 bit) kullanılarak DES şifrelemesi yapılır.
- Sonuç olarak, üç kez tekrarlanan bu işlemler sonucunda orijinal veri şifrelenmiş ve ardından çözülmüş olur.

Bu şema, verinin 64 bit olduğunu ve anahtarların da 64 bit olduğunu göstermektedir. Ancak 3DES, farklı anahtar ve veri boyutlarında da kullanılabilir. Anahtar ve veri boyutları uygulama tarafından belirlenir.

