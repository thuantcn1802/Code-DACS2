<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hotel Booking</title>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="../CSS/Index2.css">
  <link rel="stylesheet" href="../CSS/Index.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.0/css/all.min.css" integrity="sha512-9xKTRVabjVeZmc+GUW8GgSmcREDunMM+Dt/GrzchfN8tkwHizc5RP4Ok/MXFFy5rIjJjzhndFScTceq5e6GvVQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />

  <link href="https://fonts.googleapis.com/css2?family=Bungee+Shade&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Sedgwick+Ave&display=swap" rel="stylesheet">
  <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
</head>
<body>
  <!-- Header -->
  <nav class="navbar navbar-expand-lg sticky-top">
    <a class="navbar-brand" href="#">The Alpha Hotel</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Rooms</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Contact</a></li>
      </ul>
      <div class="ml-3">
        <a href="Login.html" class="btn btn-outline-primary btn-sm mr-2">Login</a>
        <a href="Register.html" class="btn btn-outline-primary btn-sm mr-2">Sign Up</a>
      </div>
    </div>
  </nav>

  <!-- Banner -->
  <div id="bannerCarousel" class="carousel slide" data-ride="carousel" data-interval="3000">
    <!-- Indicators (Optional, hiển thị chấm tròn để chuyển slide) -->
    <ol class="carousel-indicators">
      <li data-target="#bannerCarousel" data-slide-to="0" class="active"></li>
      <li data-target="#bannerCarousel" data-slide-to="1"></li>
      <li data-target="#bannerCarousel" data-slide-to="2"></li>
    </ol>

    <div class="carousel-inner">
      <!-- Slide 1 -->
      <div class="carousel-item active">
        <img src="../image/banner1.jpg" class="d-block w-100" alt="Slide 1">
        <div class="carousel-caption d-none d-md-block">
          <h1>Welcome to Our Hotel</h1>
          <p>Experience Luxury Like Never Before</p>
          <a href="#formBooking" class="btn btn-primary">Book Now</a>
        </div>
      </div>
      <!-- Slide 2 -->
      <div class="carousel-item">
        <img src="../image/banner2.jpg" class="d-block w-100" alt="Slide 2">
        <div class="carousel-caption d-none d-md-block">
          <h1>Relax in Comfort</h1>
          <p>Discover Our Premium Services</p>
          <a href="#rooms" class="btn btn-secondary">View Rooms</a>
        </div>
      </div>
      <!-- Slide 3 -->
      <div class="carousel-item">
        <img src="../image/banner3.jpg" class="d-block w-100" alt="Slide 3">
        <div class="carousel-caption d-none d-md-block">
          <h1>Exclusive Offers</h1>
          <p>Book Now and Save Big</p>
          <a href="#offers" class="btn btn-warning">Explore Deals</a>
        </div>
      </div>
    </div>

    <!-- Controls -->
    <a class="carousel-control-prev" href="#bannerCarousel" role="button" data-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#bannerCarousel" role="button" data-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>

  <!-- Booking Form -->
  <section id="formBooking" class="py-5">
    <div class="text-center mb-4" style="margin-bottom: 40px !important;;">
      <p class="first_booking">Ngồi tại nhà, bạn lựa chọn, chúng tôi tìm, chúng ta tiết kiệm.</p>
    </div>
    <div class="container">

      <div>
          <p class="info-text" style="font-weight: bold; font-size: 20px">
              Bạn muốn tìm phòng như thế nào?
          </p>
          <p class="info-text" style="margin-bottom: 20px;" >
              Hãy chọn thông tin, chúng tôi sẽ giúp bạn.
          </p>
      </div>

      <form class="form-row">
        <!-- Check-in Date -->
        <div class="form-group col-md-3">
        <button class="btn-custom">
          <span class="d-flex">
            <!-- Cột bên trái chứa icon -->
            <span class="col-md-6 d-flex justify-content-center align-items-center bg-light border">
              <i class='bx bx-calendar' ></i>
            </span>

            <!-- Cột bên phải chứa nội dung -->
            <span class="col-md-6 bg-light border">
              <span class="d-flex flex-column">
                <!-- Hàng trên cùng chứa label -->
                <span class="mb-2">
                  <label>Check-in Date</label>
                </span>
                <!-- Hàng dưới chứa input -->
                <span>
                  <input type="date" class="form-control">
                </span>
              </span>
            </span>
          </span>
        </button>
        </div>

        <!-- Check-out Date -->
        <div class="form-group col-md-3">
        <button class="btn-custom">
          <span class="d-flex">
            <!-- Cột bên trái chứa icon -->
            <span class="col-md-6 d-flex justify-content-center align-items-center bg-light border">
              <i class='bx bx-calendar-x'></i>
            </span>

            <!-- Cột bên phải chứa nội dung -->
            <span class="col-md-6 bg-light border">
              <span class="d-flex flex-column">
                <!-- Hàng trên cùng chứa label -->
                <span class="mb-2">
                  <label>Check-out Date</label>
                </span>
                <!-- Hàng dưới chứa input -->
                <span>
                  <input type="date" class="form-control">
                </span>
              </span>
            </span>
          </span>
        </button>
        </div>

        <!-- Guests -->
        <div class="form-group col-md-3">
          <button class="btn-custom">
            <span class="d-flex">
              <!-- Cột bên trái chứa icon -->
              <span class="col-md-6 d-flex justify-content-center align-items-center bg-light border">
                <i class='bx bx-user'></i>
              </span>

              <!-- Cột bên phải chứa nội dung -->
              <span class="col-md-6 bg-light border">
                <span class="d-flex flex-column">
                  <!-- Hàng trên cùng chứa label -->
                  <span class="mb-2">
                    <label>Guests</label>
                  </span>
                  <!-- Hàng dưới chứa input -->
                  <span>
                    <input type="number" class="form-control" placeholder="1">
                  </span>
                </span>
              </span>
            </span>
          </button>
        </div>

        <div class="form-group col-md-3">
          <button class="btn-custom" style="background-color: #ebebeb !important; width: 125px">
            <span class="d-flex">
              <!-- Cột bên trái (có thể chứa icon, nếu muốn) -->
              <span class="col-md-6 d-flex justify-content-center align-items-center bg-light border" style="flex: 0 0 25%; max-width: 25%;">
                <i class='bx bx-search'></i> <!-- Icon tìm kiếm -->
              </span>

              <!-- Cột bên phải chứa nội dung -->
              <span class="col-md-6 bg-light border" style="flex: 1; max-width: 75%;">
                Search
              </span>
            </span>
          </button>
        </div>
      </form>
    </div>
  </section>

  <!-- Rooms Section -->
  <section id="rooms" class="py-5">
    <div class="text-center mb-4">
      <p class="first_booking">Tham khảo phòng ở của chúng tôi</p>
    </div>
    <div class="container-rooms">
      <div class="slide">
              <div class="item" style="background-image: url(../image/room1.jpg);">
                  <div class="content">
                      <div class="name">Room 1</div>
                      <div class="des">Cao, rộng, thoáng mát</div>
                      <button>See More</button>  
                  </div>
              </div> 
              
              <div class="item" style="background-image: url(../image/room2.jpg);">
                  <div class="content">
                      <div class="name">Room 2</div>
                      <div class="des">Cao, rộng, ấm áp</div>
                      <button>See More</button>
                  </div>
              </div>
              
              <div class="item" style="background-image: url(../image/room3.jpg);">
                  <div class="content">
                      <div class="name">Room 3</div>
                      <div class="des">Sạch sẽ, rộng rãi, sáng sủa</div>
                      <button>See More</button>
                  </div>
              </div> 

              <div class="item" style="background-image: url(../image/room4.jpg);">
                  <div class="content">
                      <div class="name">Room 4</div>
                      <div class="des">Mộng mơ, tone dịu dàng, thơm mát</div>
                      <button>See More</button>
                  </div>
              </div> 

              <div class="item" style="background-image: url(../image/room5.jpg);">
                  <div class="content">
                      <div class="name">Room 5</div>
                      <div class="des">Mát mẻ, gần gũi với thiên nhiên, trong lành</div>
                      <button>See More</button>
                  </div>
              </div> 

              <div class="item" style="background-image: url(../image/room6.jpg);">
                  <div class="content">
                      <div class="name">Room 6</div>
                      <div class="des">Ly kì, bí ẩn, mơ mộng</div>
                      <button>See More</button>
                  </div>
              </div> 

              <div class="item" style="background-image: url(../image/room7.jpg);">
                  <div class="content">
                      <div class="name">Room 7</div>
                      <div class="des">Cao cấp, xịn xò, vip</div>
                      <button>See More</button>
                  </div>
              </div> 

              <div class="item" style="background-image: url(../image/room8.jpg);">
                  <div class="content">
                      <div class="name">Room 8</div>
                      <div class="des">Hiện đại, đẹp mắt, tinh xảo</div>
                      <button>See More</button>
                  </div>
              </div> 
          </div> 

          <div class="button">
              <button class="prev"><i class="fa-solid fa-arrow-left"></i></button>
              <button class="next"><i class="fa-solid fa-arrow-right"></i></button>
          </div>
      </div>
  </section>

  <!-- Phần Thống Kê với Biểu Đồ -->
  <section id="statistics" class="py-5">
    <div class="text-center mb-4">
    <p class="first_booking">Thống Kê Đặt Phòng</p>
    </div>
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <canvas id="bookingChart"></canvas>
          </div>
        </div>
      </div> 
  </section>

  <!-- Tiện ích -->
  <section id="benefits" class="py-5 bg-light">
    <div class="text-center mb-4">
      <p class="first_booking" style="margin: 0 0 40px;">Lợi thế của chúng tôi</p>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <div class="card">
            <img src="../image/SearchDesktop.jpg" class="card-img-top" alt="Benefit 1">
            <div class="card-body">
              <h5 class="card-title">Đặt Phòng Dễ Dàng</h5>
              <p class="card-text">Tìm và đặt phòng khách sạn chỉ trong vài giây.</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card">
            <img src="../image/CompareDesktop.jpg" class="card-img-top" alt="Benefit 2">
            <div class="card-body">
              <h5 class="card-title">Tự tin về chất lượng</h5>
              <p class="card-text">Số 1 về không gian phòng ở, chất lượng dịch vụ và sự hài lòng của khách hàng.<p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card">
            <img src="../image/SaveDesktop.jpg" class="card-img-top" alt="Benefit 3">
            <div class="card-body">
              <h5 class="card-title">Nhiều ưu đãi</h5>
              <p class="card-text">Cơ hội nhận được nhiều ưu đãi, quà tặng cực chất, siêu ngầu.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-dark text-white py-4">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <h5>Contact Us</h5>
          <p>
            Da Nang City<br>
            Email: thealphahotel@hotel.com<br>
            Phone: +84 123 456 789
          </p>
        </div>
        <div class="col-md-3">
          <h5>Quick Links</h5>
          <ul class="list-unstyled">
            <li><a href="#" class="text-white">Home</a></li>
            <li><a href="#" class="text-white">Rooms</a></li>
          </ul>
        </div>
        <div class="col-md-3">
          <h5>Follow Us</h5>
          <a href="#" class="text-white mr-2"><i class="fab fa-facebook"></i></a>
          <a href="#" class="text-white"><i class="fab fa-instagram"></i></a>
        </div>
        <div class="col-md-3">
          <h5>Newsletter</h5>
          <form>
            <input type="email" class="form-control" placeholder="Your Email">
            <button class="btn btn-primary btn-block mt-2">Subscribe</button>
          </form>
        </div>
      </div>
    </div>
  </footer>

  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.4.4/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script src="../Script/thongke.js"></script>
  <script src="../Script/laynen.js"></script>
</body>
</html>
