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
    <li class="fragment fade-left">Object Storage</li>
    <li class="fragment fade-left">S3 Storage</li>
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
     <li style="color: gray;">Object Storage</li>
     <li style="color: gray;">S3 Storage</li>
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
      <h3>Storage for the internet</h3>
      <p><span class="fragment">Đa dạng hóa trong việc lưu trữ dữ liệu như tốc độ, nền tảng, kiểu dữ liệu, ..</span></p>
      <p><span class="fragment">Năm 2006, Amazon công bố S3 Object Storage</span></p>
    </div>
    <aside class="notes">
      Cách mạng công nghiệp lần 4
      APIs, IoT, AI, ..
    </aside>
  </section>
</section>
<!-- END 1 -->

<!-- 2 -->
<section id="fragments">
  <section>
    <h1>MỤC LỤC</h1>
    <ul>
     <li style="color: gray;">Giới thiệu về S3 Storage</li>
     <li><b>Object Storage</b></li>
     <li style="color: gray;">S3 Storage</li>
     <li style="color: gray;">Các nhà cung cấp S3</li>
     <li style="color: gray;">VNDATA Cloud Object Storage project</li>
    </ul>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/009.png" data-background-size="100%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h2>Object Storage và các Storage truyền thống</h2>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/009.png" data-background-size="100%">
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/010.jpeg" data-background-size="85%">
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/011.jpg" data-background-size="85%">
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/012.jpg" data-background-size="85%">
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/013.jpg" data-background-size="85%">
  </section>
</section>
<!-- END 2 -->

<!-- 3 -->
<section id="fragments">
  <section>
    <h1>MỤC LỤC</h1>
    <ul>
     <li style="color: gray;">Giới thiệu về S3 Storage</li>
     <li style="color: gray;">Object Storage</li>
     <li><b>S3 Storage</b></li>
     <li style="color: gray;">Các nhà cung cấp S3</li>
     <li style="color: gray;">VNDATA Cloud Object Storage project</li>
    </ul>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/014.jpg" data-background-size="90%">
    <br><br><br><br>
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>S<span style="color: gray;">imple</span> S<span style="color: gray;">torage</span> S<span style="color: gray;">ervice</span></h3>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/014.jpg" data-background-size="90%">
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <p class="fragment"><span style="color: gray;">Amazon Simple Storage Service (S3) is a</span> storage for the internet.</p>
      <p class="fragment"><span style="color: gray;">It is designed for </span>large-capacity, low-cost storage <span style="color: gray;">provision</span> across multiple geographical regions.</p>
      <p class="fragment"><span style="color: gray;">Amazon S3 provides developers and IT teams with</span> Secure, Durable <span style="color: gray;">and</span> Highly Scalable <span style="color: gray;">object storage.</span></p>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/015.jpeg" data-background-size="80%">
    <br><br><br><br>
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Storage for the internet</h3>
      <ul>
        <li class="fragment">Có thể truy cập từ mọi nơi trên Internet</li>
        <li class="fragment">Lưu trữ được nhiều loại dữ liệu</li>
        <li class="fragment">Đa nền tảng</li>
        <li class="fragment">Đa ứng dụng</li>
        <li class="fragment">Tương thích với các loại Storages khác</li>
       </ul>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/016.jpeg" data-background-size="80%">
    <br><br><br><br>
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Large-capacity Storage</h3>
      <ul>
        <li class="fragment">Dung lượng lưu trữ cực lớn được nhà cung cấp tính toán</li>
        <li class="fragment">Khách hàng chủ động mở rộng dung lượng sử dụng không giới hạn</li>
       </ul>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/017.jpg" data-background-size="70%">
    <br><br><br><br>
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Low-cost Storage</h3>
      <ul>
        <li class="fragment">Pay-as-you-go</li>
        <li class="fragment">Khách hàng chủ động giảm dung lượng sử dụng</li>
       </ul>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/018.png" data-background-size="80%">
    <br><br><br><br>
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Across multiple geographical regions</h3>
      <ul>
        <li class="fragment">Tương thích với đa số các nhà cung cấp CDN</li>
        <li class="fragment">Cấu hình storage tương ứng với vị trí địa lý</li>
       </ul>
    </div>
  </section>
  <section data-background="{{site.baseurl}}/images/2022/10/08/s3-storage-cloudian/019.png" data-background-size="80%">
    <br><br><br><br>
    <div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; opacity: 0.9;">
      <h3>Secure, Durable and Highly Scalable</h3>
      <ul>
        <li class="fragment">Mã hóa dữ liệu ở client và server side</li>
        <li class="fragment">Có nhiều bản copy để phục hồi dữ liệu</li>
        <li class="fragment">Sử dụng checksum để xác minh tính toàn vẹn dữ liệu</li>
       </ul>
    </div>
  </section>
</section>
<!-- END 3 -->

<!-- 4 -->
<section id="fragments">
  <section>
    <h1>MỤC LỤC</h1>
    <ul>
     <li style="color: gray;">Giới thiệu về S3 Storage</li>
     <li style="color: gray;">Object Storage</li>
     <li style="color: gray;">S3 Storage</li>
     <li><b>Các nhà cung cấp S3</b></li>
     <li style="color: gray;">VNDATA Cloud Object Storage project</li>
    </ul>
  </section>
</section>
<!-- 4 -->

<!-- 5 -->
<section id="fragments">
  <section>
    <h1>MỤC LỤC</h1>
    <ul>
     <li style="color: gray;">Giới thiệu về S3 Storage</li>
     <li style="color: gray;">Object Storage</li>
     <li style="color: gray;">S3 Storage</li>
     <li style="color: gray;">Các nhà cung cấp S3</li>
     <li><b>VNDATA Cloud Object Storage project</b></li>
    </ul>
  </section>
</section>
<!-- 5 -->