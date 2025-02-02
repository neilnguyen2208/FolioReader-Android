# Vietnamese version FolioReader 0.5.4 - 11
- Phiên bản nâng cấp tiếng Việt từ thư viện FolioReader-Android 0.5.4
+ FolioReader-Android is an EPUB reader written in Java and Kotlin. See the [FOLIOREADER_PROJECT](https://github.com/FolioReader/FolioReader-Android) .
+ FolioReaderKit is available under the BSD license. See the [LICENSE](https://github.com/FolioReader/FolioReader-Android/blob/master/License.md) file.

[![](https://jitpack.io/v/dongnvsince1999/FolioReader-Android.svg)](https://jitpack.io/#dongnvsince1999/FolioReader-Android)

### Các tính năng của FolioReader 0.5.4 + Demo: [FOLIOREADER_PROJECT](https://github.com/FolioReader/FolioReader-Android) .

### Các tính năng của phiên bản nâng cấp Tiếng Việt:
- Xử lý Internal / External links
- Portrait / Landscape
- Themes / Day mode / Night mode
- Highlight
- Tìm kiếm trong sách.
- Cập nhật ngôn ngữ tiếng Việt.
- Thay đổi toàn bộ giao diện.
- Custom Fonts cho tài liệu Tiếng Việt.
- Custom Textsize
- Thay đổi màu trong List / Edit / Delete Highlights.
- Hỗ trợ dịch từ trực tiếp trong ứng dụng.
- Hỗ trợ từ điển tiếng Việt offline.
- Bỏ tính năng share.
- Last ReadLocator
- Horizontal Reading
- Cập nhật ngôn ngữ Turkey
## Demo:

### Đọc sách:

![alt text](https://raw.githubusercontent.com/dongnvsince1999/FolioReader-Android/master/folioreader/readbook.png)

### Thao tác với từ ngữ trong sách:

![alt text](https://raw.githubusercontent.com/dongnvsince1999/FolioReader-Android/master/folioreader/show.png)

### Quản lý mục lục và ghi chú:

![alt text](https://raw.githubusercontent.com/dongnvsince1999/FolioReader-Android/master/folioreader/contenthighlight.png)

### Thay đổi font, cỡ chữ, chế độ ngày / đêm:

![alt text](https://raw.githubusercontent.com/dongnvsince1999/FolioReader-Android/master/folioreader/nightmode.png)

### Tìm kiếm trong sách:

![alt text](https://raw.githubusercontent.com/dongnvsince1999/FolioReader-Android/master/folioreader/search.png)

## Hướng dẫn các dependence:

Thêm dependency vào root project `build.gradle` file:

```groovy
allprojects {
    repositories {
        ...
        jcenter()
        maven { url "https://jitpack.io" }
        ...
    }
}
```

Thêm dependency vào app module `build.gradle` file:

```groovy
dependencies {
    ...
	     implementation 'com.github.dongnvsince1999:FolioReader-Android:0.5.4-10'
    ...
}
```


## Hướng dẫn sử dụng:

Lấy singleton object `FolioReader`:

```java
FolioReader folioReader = FolioReader.get();
```

Gọi hàm `openBook()`:

##### opening from file path:

```java
folioReader.openBook("/sdcard/Download/Book.epub");
```
##### opening book from assets -

```java
folioReader.openBook("file:///android_asset/TheSilverChair.epub");
```
##### opening book from raw -

```java
folioReader.openBook(R.raw.accessible_epub_3);
```

## Đây là bản mở rộng của Folio Reader, mọi thông tin về Folio Reader có thể tham khảo tại: [FOLIOREADER_PROJECT](https://github.com/FolioReader/FolioReader-Android)

### Tác giả của FolioReader-Android:
[**Heberti Almeida**](https://github.com/hebertialmeida)

- **Twitter**: [**@hebertialmeida**](https://twitter.com/hebertialmeida)
- **LinkedIn**: [**hebertialmeida**](http://linkedin.com/in/hebertialmeida)

## Các tham khảo khác:
 - FOLIOREADER WIKI
 - [**EPUB CFI**](http://idpf.org/epub/linking/cfi/epub-cfi.html)
 - [**Rangy**](https://github.com/timdown/rangy)
 - API của Dịch từ của Google: translate.googleapis.com
 - Data từ điển được lấy và convert từ [**UNDERTHESEAPROJECT**](https://github.com/undertheseanlp/underthesea)(Github)
