---
title: S3 Storage (Cloudian)
layout: post
theme: black
---
<!-- TITLE -->
<section>
  <h1>S3 STORAGE</h1>
  <h3>Giới thiệu về S3 Storage & <br> VNDATA Cloud Object Storage project</h3>
  <p style="text-align: right;">
    <small><b>Author:</b> TraiOi</small><br />
    <small><b>Company:</b> VNDATA</small>
  </p>
</section>
<!-- END TITLE -->

<!-- MUCLUC -->
<section id="fragments">
  <h1>MỤC LỤC</h1>
  <ul>
    <li class="fragment fade-left">Giới thiệu về S3 Storage</li>
    <li class="fragment fade-left">Các tính năng và mô hình cơ bản</li>
    <li class="fragment fade-left">Ưu điểm và Khuyết điểm</li>
    <li class="fragment fade-left">Ứng dụng</li>
    <li class="fragment fade-left">Các nhà cung cấp S3</li>
    <li class="fragment fade-left">VNDATA Cloud Object Storage project</li>
  </ul>
</section>
<!-- END MUCLUC -->

<!-- 1 -->
<section id="fragments">
  <section>
    <h1>MỤC LỤC</h1>
    <ul>
     <li><b>Giới thiệu về S3 Storage</b></li>
     <li style="color: gray;">Các tính năng và mô hình cơ bản</li>
     <li style="color: gray;">Ưu điểm và Khuyết điểm</li>
     <li style="color: gray;">Ứng dụng</li>
     <li style="color: gray;">Các nhà cung cấp S3</li>
     <li style="color: gray;">VNDATA Cloud Object Storage project</li>
    </ul>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/001.jpg" data-background-size="80%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h2>Sự phát triển của Data Storage</h2>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/002.jpg" data-background-size="50%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Trước thế kỷ 18 ..</h3>
      <p><span class="fragment">Con người đã nghĩ ra cách backup dữ liệu bằng cách sao chép các thông tin quan trọng</span><span class="fragment"> vào giấy</span></p>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/003.jpg" data-background-size="90%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Kỷ nguyên dữ liệu số</h3>
      <p><span class="fragment">Năm 1832, Korsakov đã sử dụng các <b>punched cards</b> trong lưu trữ và tìm kiếm thông tin</span></p>
      <p><span class="fragment">Năm 1890, Herman Hollerith đã phát triển 1 phương pháp để máy móc ghi và lưu dữ liệu giúp điều tra dân số Hoa Kỳ trên <b>punched cards</b></span></p>
      <p><span class="fragment">Sau đó, ông thành lập công ty được biết với tên IBM</span></p>
    </div>
    <aside class="notes">
      Cách mạng công nghiệp lần thứ 2
    </aside>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/004.jpg" data-background-size="90%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Cách mạng kỹ thuật số</h3>
      <p><span class="fragment">Năm 1951, IBM phát triển được hệ thống máy tính lưu trữ dữ liệu số</span></p>
      <p><span class="fragment">Đĩa từ (magnetic tape) ra đời</span></p>
    </div>
    <aside class="notes">
      Cách mạng công nghiệp lần thứ 3
    </aside>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/005.jpg" data-background-size="70%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>HDD đầu tiên</h3>
      <p><span class="fragment">Năm 1956, IBM phát minh Hard Disk Drive (HDD) đầu tiên</span></p>
      <p><span class="fragment">Lúc này HDD chỉ có thể lưu được 10MB dữ liệu</span></p>
    </div>
    <aside class="notes">
      Cách mạng công nghiệp lần thứ 3
    </aside>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/006.jpg" data-background-size="80%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Sự thay đổi về tốc độ</h3>
      <p><span class="fragment">Năm 1996, M-system giới thiệu một ổ đĩa SSD dựa trên công nghệ bộ nhớ flash</span></p>
      <p><span class="fragment">với tốc độ vượt xa HDD truyền thống</span></p>
      <p><span class="fragment">nhưng giá thành rất cao</span></p>
    </div>
    <aside class="notes">
      (được SanDisk mua lại năm 2006)
      Solid-state ổ đĩa bán dẫn
      Flaskdisk = SSD
    </aside>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/007.jpg" data-background-size="70%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Công nghệ điện toán đám mây</h3>
      <p><span class="fragment">1990s, các công ty công nghệ tiếp tục công bố Cloud Storage:</span></p>
      <p><span class="fragment">Apple (iCloud)</span></p>
      <p><span class="fragment">Amazon (Amazon Web Services)</span></p>
      <p><span class="fragment">Dropbox (Dropbox)</span></p>
      <p><span class="fragment">Google (Google Drive)</span></p>
    </div>
    <aside class="notes">
      
    </aside>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/008.png" data-background-size="100%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Cách mạng công nghiệp lần 4</h3>
      <p><span class="fragment">Năm 2006, Amazon công bố S3 Object Storage</span></p>
      <p><span class="fragment">Đa dạng hóa trong việc lưu trữ dữ liệu như tốc độ, nền tảng, kiểu dữ liệu, ..</span></p>
    </div>
    <aside class="notes">
      APIs, IoT, AI, ..
    </aside>
  </section>
</section>
<!-- END 1 -->