<nav class="navbar">
<div class="nav">
    <img src="img/dark-logo.png" class="brand-logo" alt="">
    <div class="nav-items">
        <div class="search">
            <input type="text" class="search-box" placeholder="search brand, product">
            <button class="search-btn">search</button>
        </div>
        <a href="#"><img src="img/user.png" alt=""></a>
        <a href="#"><img src="img/cart.png" alt=""></a>
    </div>
</div>
</nav>
Open home.css file. And inside it befo
@import 'nav.css';
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'roboto', sans-serif;
}

.navbar{
    position: sticky;
    top: 0;
    left: 0;
    width: 100%;
    background: #f5f5f5;
    z-index: 9;
}

.nav{
    padding: 10px 10vw;
    display: flex;
    justify-content: space-between;
}

.brand-logo{
    height: 60px;
}

.nav-items{
    display: flex;
    align-items: center;
}

.search{
    width: 500px;
    display: flex;
}

.search-box{
    width: 80%;
    height: 40px;
    padding: 10px;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
    border: 1px solid #d1d1d1;
    text-transform: capitalize;
    background: none;
    color: #a9a9a9;
    outline: none;
}

.search-btn{
    width: 20%;
    height: 40px;
    padding: 10px 20px;
    border: none;
    outline: none;
    cursor: pointer;
    background: #383838;
    color: #fff;
    text-transform: capitalize;
    font-size: 15px;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
}

.search-box::placeholder{
    color: #a9a9a9;
}

.nav-items a{
    margin-left: 20px;
}

.nav-items a img{
    width: 30px;
}
<ul class="links-container">
    <li class="link-item"><a href="#" class="link">home</a></li>
    <li class="link-item"><a href="#" class="link">women</a></li>
    <li class="link-item"><a href="#" class="link">men</a></li>
    <li class="link-item"><a href="#" class="link">kids</a></li>
    <li class="link-item"><a href="#" class="link">accessories</a></li>
</ul>
.links-container{
    width: 100%;
    display: flex;
    padding: 10px 10vw;
    justify-content: center;
    list-style: none;
    border-top: 1px solid #d1d1d1;
}

.link{
    text-transform: capitalize;
    padding: 0 10px;
    margin: 0 5px;
    text-decoration: none;
    color: #383838;
    opacity: 0.5;
    transition: .5s;
}

.link:hover{
    opacity: 1;
}
const createNav = () => {
    let nav = document.querySelector('.navbar');

    nav.innerHTML = `
        <div class="nav">
            <img src="img/dark-logo.png" class="brand-logo" alt="">
            <div class="nav-items">
                <div class="search">
                    <input type="text" class="search-box" placeholder="search brand, product">
                    <button class="search-btn">search</button>
                </div>
                <a href="#"><img src="img/user.png" alt=""></a>
                <a href="#"><img src="img/cart.png" alt=""></a>
            </div>
        </div>
        <ul class="links-container">
            <li class="link-item"><a href="#" class="link">home</a></li>
            <li class="link-item"><a href="#" class="link">women</a></li>
            <li class="link-item"><a href="#" class="link">men</a></li>
            <li class="link-item"><a href="#" class="link">kids</a></li>
            <li class="link-item"><a href="#" class="link">accessories</a></li>
        </ul>
    `;
}

createNav();
<nav class="navbar"></nav>
<script src="js/nav.js"></script>
<!-- hero section -->
<header class="hero-section">
    <div class="content">
        <img src="img/light-logo.png" class="logo" alt="">
        <p class="sub-heading">best fashion collection of all time</p>
    </div>
</header>
@import 'nav.css';

.hero-section{
    width: 100%;
    height: calc(100vh - 120px);
    background-image: url('../img/header.png');
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
}

.hero-section .logo{
    height: 150px;
    display: block;
    margin: auto;
}

.hero-section .sub-heading{
    margin-top: 10px;
    text-align: center;
    color: #fff;
    text-transform: capitalize;
    font-size: 35px;
    font-weight: 300;
}
<section class="product">
    <h2 class="product-category">best selling</h2>
</section>
.product{
    position: relative;
    overflow: hidden;
    padding: 20px 0;
}

.product-category{
    padding: 0 10vw;
    font-size: 30px;
    font-weight: 500;
    margin-bottom: 40px;
    text-transform: capitalize;
}
// inside product section.
<div class="product-container">
    <div class="product-card">
        <div class="product-image">
            <span class="discount-tag">50% off</span>
            <img src="img/card1.png" class="product-thumb" alt="">
            <button class="card-btn">add to whislist</button>
        </div>
        <div class="product-info">
            <h2 class="product-brand">brand</h2>
            <p class="product-short-des">a short line about the cloth..</p>
            <span class="price">$20</span><span class="actual-price">$40</span>
        </div>
    </div>
    +7 more cards
</div>
.product-container{
    padding: 0 10vw;
    display: flex;
    overflow-x: auto;
    scroll-behavior: smooth;
}

.product-container::-webkit-scrollbar{
    display: none;
}

.product-card{
    flex: 0 0 auto;
    width: 250px;
    height: 450px;
    margin-right: 40px;
}

.product-image{
    position: relative;
    width: 100%;
    height: 350px;
    overflow: hidden;
}

.product-thumb{
    width: 100%;
    height: 350px;
    object-fit: cover;
}

.discount-tag{
    position: absolute;
    background: #fff;
    padding: 5px;
    border-radius: 5px;
    color: #ff7d7d;
    right: 10px;
    top: 10px;
    text-transform: capitalize;
}

.card-btn{
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    padding: 10px;
    width: 90%;
    text-transform: capitalize;
    border: none;
    outline: none;
    background: #fff;
    border-radius: 5px;
    transition: 0.5s;
    cursor: pointer;
    opacity: 0;
}

.product-card:hover .card-btn{
    opacity: 1;
}

.card-btn:hover{
    background: #efefef;
}

.product-info{
    width: 100%;
    height: 100px;
    padding-top: 10px;
}

.product-brand{
    text-transform: uppercase;
}

.product-short-des{
    width: 100%;
    height: 20px;
    line-height: 20px;
    overflow: hidden;
    opacity: 0.5;
    text-transform: capitalize;
    margin: 5px 0;
}

.price{
    font-weight: 900;
    font-size: 20px;
}

.actual-price{
    margin-left: 20px;
    opacity: 0.5;
    text-decoration: line-through;
}
// before product-container element.
<button class="pre-btn"><img src="img/arrow.png" alt=""></button>
<button class="nxt-btn"><img src="img/arrow.png" alt=""></button>
.pre-btn, .nxt-btn{
    border: none;
    width: 10vw;
    height: 100%;
    position: absolute;
    top: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(90deg, rgba(255, 255, 255, 0) 0%, #fff 100%);
    cursor: pointer;
    z-index: 8;
}

.pre-btn{
    left: 0;
    transform: rotate(180deg);
}

.nxt-btn{
    right: 0;
}

.pre-btn img, .nxt-btn img{
    opacity: 0.2;
}

.pre-btn:hover img, .nxt-btn:hover img{
    opacity: 1;
}
const productContainers = [...document.querySelectorAll('.product-container')];
const nxtBtn = [...document.querySelectorAll('.nxt-btn')];
const preBtn = [...document.querySelectorAll('.pre-btn')];

productContainers.forEach((item, i) => {
    let containerDimenstions = item.getBoundingClientRect();
    let containerWidth = containerDimenstions.width;

    nxtBtn[i].addEventListener('click', () => {
        item.scrollLeft += containerWidth;
    })

    preBtn[i].addEventListener('click', () => {
        item.scrollLeft -= containerWidth;
    })
})
<script src="js/home.js"></script>
<!-- collections -->
<section class="collection-container">
    <a href="#" class="collection">
        <img src="img/women-collection.png" alt="">
        <p class="collection-title">women <br> apparels</p>
    </a>
    <a href="#" class="collection">
        <img src="img/men-collection.png" alt="">
        <p class="collection-title">men <br> apparels</p>
    </a>
    <a href="#" class="collection">
        <img src="img/accessories-collection.png" alt="">
        <p class="collection-title">accessories</p>
    </a>
</section>
.collection-container{
    width: 100%;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 10px;
}

.collection{
    position: relative;
}

.collection img{
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.collection p{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    color: #fff;
    font-size: 50px;
    text-transform: capitalize;
}

.collection:nth-child(3){
    grid-column: span 2;
    margin-bottom: 10px;
}
<footer>
    <div class="footer-content">
        <img src="img/light-logo.png" class="logo" alt="">
        <div class="footer-ul-container">
            <ul class="category">
                <li class="category-title">men</li>
                <li><a href="#" class="footer-link">t-shirts</a></li>
                <li><a href="#" class="footer-link">sweatshirts</a></li>
                <li><a href="#" class="footer-link">shirts</a></li>
                <li><a href="#" class="footer-link">jeans</a></li>
                <li><a href="#" class="footer-link">trousers</a></li>
                <li><a href="#" class="footer-link">shoes</a></li>
                <li><a href="#" class="footer-link">casuals</a></li>
                <li><a href="#" class="footer-link">formals</a></li>
                <li><a href="#" class="footer-link">sports</a></li>
                <li><a href="#" class="footer-link">watch</a></li>
            </ul>
            <ul class="category">
                <li class="category-title">women</li>
                <li><a href="#" class="footer-link">t-shirts</a></li>
                <li><a href="#" class="footer-link">sweatshirts</a></li>
                <li><a href="#" class="footer-link">shirts</a></li>
                <li><a href="#" class="footer-link">jeans</a></li>
                <li><a href="#" class="footer-link">trousers</a></li>
                <li><a href="#" class="footer-link">shoes</a></li>
                <li><a href="#" class="footer-link">casuals</a></li>
                <li><a href="#" class="footer-link">formals</a></li>
                <li><a href="#" class="footer-link">sports</a></li>
                <li><a href="#" class="footer-link">watch</a></li>
            </ul>
        </div>
    </div>
</footer>
@import 'nav.css';
@import 'footer.css';
footer{
    position: relative;
    width: 100%;
    padding: 40px 10vw;
    padding-bottom: 80px;
    background: #383838;
}

.footer-content{
    display: flex;
    width: 100%;
    justify-content: space-between;
}

.footer-content .logo{
    height: 160px;
}

.footer-ul-container{
    width: 45%;
    display: flex;
    justify-content: space-between;
}

.category{
    width: 200px;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 10px;
    list-style: none;
}

.category-title{
    grid-column: span 2;
    text-transform: capitalize;
    color: #fff;
    font-size: 20px;
    margin-bottom: 20px;
}

.category .footer-link{
    text-decoration: none;
    text-transform: capitalize;
    color: rgba(255, 255, 255, 0.75);
}

.footer-link:hover{
    color: #fff;
}
<footer>
    // previous elements
    <p class="footer-title">about company</p>
    <p class="info">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellat tempore ad suscipit, eos eius quisquam sed optio nisi quaerat fugiat ratione et vero maxime praesentium, architecto minima reiciendis iste quo deserunt assumenda alias ducimus. Ullam odit maxime id voluptates rerum tenetur corporis laboriosam! Cum error ipsum laborum tempore in rerum necessitatibus nostrum nobis modi! Debitis adipisci illum nemo aperiam sed, et accusamus ut officiis. Laborum illo exercitationem quo culpa reprehenderit excepturi distinctio tempore cupiditate praesentium nisi ut iusto, assumenda perferendis facilis voluptas autem fuga sunt ab debitis voluptatum harum eum. Asperiores, natus! Est deserunt incidunt quasi placeat omnis, itaque harum?</p>
    <p class="info">support emails - help@clothing.com, customersupport@clothing.com</p>
    <p class="info">telephone - 180 00 00 001, 180 00 00 002</p>
    <div class="footer-social-container">
        <div>
            <a href="#" class="social-link">terms & services</a>
            <a href="#" class="social-link">privacy page</a>
        </div>
        <div>
            <a href="#" class="social-link">instagram</a>
            <a href="#" class="social-link">facebook</a>
            <a href="#" class="social-link">twitter</a>
        </div>
    </div>
    <p class="footer-credit">Clothing, Best apparels online store</p>
</footer>
.footer-title, .info{
    color: rgba(255, 255, 255, 0.75);
    margin: 20px 0;
    text-transform: capitalize;
}

.footer-title{
    margin-top: 80px;
    color: #fff;
}

.footer-social-container{
    margin-top: 40px;
    display: flex;
    justify-content: space-between;
}

.social-link{
    color: #fff;
    margin-left: 20px;
    text-transform: capitalize;
}

.social-link:nth-child(1){
    margin-left: 0;
}

.footer-credit{
    width: 100%;
    padding: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    text-align: center;
    color: #fff;
    background: rgba(0, 0, 0, 0.2);
}
const createFooter = () => {
    let footer = document.querySelector('footer');

    footer.innerHTML = `
    <div class="footer-content">
        <img src="img/light-logo.png" class="logo" alt="">
        <div class="footer-ul-container">
            <ul class="category">
                <li class="category-title">men</li>
                <li><a href="#" class="footer-link">t-shirts</a></li>
                <li><a href="#" class="footer-link">sweatshirts</a></li>
                <li><a href="#" class="footer-link">shirts</a></li>
                <li><a href="#" class="footer-link">jeans</a></li>
                <li><a href="#" class="footer-link">trousers</a></li>
                <li><a href="#" class="footer-link">shoes</a></li>
                <li><a href="#" class="footer-link">casuals</a></li>
                <li><a href="#" class="footer-link">formals</a></li>
                <li><a href="#" class="footer-link">sports</a></li>
                <li><a href="#" class="footer-link">watch</a></li>
            </ul>
            <ul class="category">
                <li class="category-title">women</li>
                <li><a href="#" class="footer-link">t-shirts</a></li>
                <li><a href="#" class="footer-link">sweatshirts</a></li>
                <li><a href="#" class="footer-link">shirts</a></li>
                <li><a href="#" class="footer-link">jeans</a></li>
                <li><a href="#" class="footer-link">trousers</a></li>
                <li><a href="#" class="footer-link">shoes</a></li>
                <li><a href="#" class="footer-link">casuals</a></li>
                <li><a href="#" class="footer-link">formals</a></li>
                <li><a href="#" class="footer-link">sports</a></li>
                <li><a href="#" class="footer-link">watch</a></li>
            </ul>
        </div>
    </div>
    <p class="footer-title">about company</p>
    <p class="info">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellat tempore ad suscipit, eos eius quisquam sed optio nisi quaerat fugiat ratione et vero maxime praesentium, architecto minima reiciendis iste quo deserunt assumenda alias ducimus. Ullam odit maxime id voluptates rerum tenetur corporis laboriosam! Cum error ipsum laborum tempore in rerum necessitatibus nostrum nobis modi! Debitis adipisci illum nemo aperiam sed, et accusamus ut officiis. Laborum illo exercitationem quo culpa reprehenderit excepturi distinctio tempore cupiditate praesentium nisi ut iusto, assumenda perferendis facilis voluptas autem fuga sunt ab debitis voluptatum harum eum. Asperiores, natus! Est deserunt incidunt quasi placeat omnis, itaque harum?</p>
    <p class="info">support emails - help@clothing.com, customersupport@clothing.com</p>
    <p class="info">telephone - 180 00 00 001, 180 00 00 002</p>
    <div class="footer-social-container">
        <div>
            <a href="#" class="social-link">terms & services</a>
            <a href="#" class="social-link">privacy page</a>
        </div>
        <div>
            <a href="#" class="social-link">instagram</a>
            <a href="#" class="social-link">facebook</a>
            <a href="#" class="social-link">twitter</a>
        </div>
    </div>
    <p class="footer-credit">Clothing, Best apparels online store</p>
    `;
}

createFooter();
<footer></footer>

<script src="js/footer.js"></script>    
<head>
    <link rel="stylesheet" href="css/home.css">
    <link rel="stylesheet" href="css/product.css">
</head>
<script src="js/nav.js"></script>
<script src="js/footer.js"></script>
<script src="js/home.js"></script>
<script src="js/product.js"></script>
<nav class="navbar"></nav>
<footer></footer>
<section class="product-details">
    <div class="image-slider">
        <div class="product-images">
            <img src="img/product image 1.png" class="active" alt="">
            <img src="img/product image 2.png" alt="">
            <img src="img/product image 3.png" alt="">
            <img src="img/product image 4.png" alt="">
        </div>
    </div>
</section>
.product-details{
    width: 100%;
    padding: 60px 10vw;
    display: flex;
    justify-content: space-between;
}

.image-slider{
    width: 500px;
    height: 500px;
    position: relative;
    background-image: url('../img/product\ image\ 1.png');
    background-size: cover;
}

.product-images{
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    width: 90%;
    background: #fff;
    border-radius: 5px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    height: 100px;
    grid-gap: 10px;
    padding: 10px;
}

.product-images img{
    width: 100%;
    height: 80px;
    object-fit: cover;
    cursor: pointer;
}

.product-images img.active{
    opacity: 0.5;
}
<section>
   // image slider
   <div class="details">
        <h2 class="product-brand">calvin klein</h2>
        <p class="product-short-des">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
        <span class="product-price">$99</span>
        <span class="product-actual-price">$200</span>
        <span class="product-discount">( 50% off )</span>

        <p class="product-sub-heading">select size</p>

        <input type="radio" name="size" value="s" checked hidden id="s-size">
        <label for="s-size" class="size-radio-btn check">s</label>
        <input type="radio" name="size" value="m" hidden id="m-size">
        <label for="m-size" class="size-radio-btn">m</label>
        <input type="radio" name="size" value="l" hidden id="l-size">
        <label for="l-size" class="size-radio-btn">l</label>
        <input type="radio" name="size" value="xl" hidden id="xl-size">
        <label for="xl-size" class="size-radio-btn">xl</label>
        <input type="radio" name="size" value="xxl" hidden id="xxl-size">
        <label for="xxl-size" class="size-radio-btn">xxl</label>

        <button class="btn cart-btn">add to cart</button>
        <button class="btn">add to wishlist</button>
    </div>
</section>
.details{
    width: 50%;
}

.details .product-brand{
    text-transform: capitalize;
    font-size: 30px;
}

.details .product-short-des{
    font-size: 25px;
    line-height: 30px;
    height: auto;
    margin: 15px 0 30px;
}

.product-price{
    font-weight: 700;
    font-size: 30px;
}

.product-actual-price{
    font-size: 30px;
    opacity: 0.5;
    text-decoration: line-through;
    margin: 0 20px;
    font-weight: 300;
}

.product-discount{
    color: #ff7d7d;
    font-size: 20px;
}

.product-sub-heading{
    font-size: 30px;
    text-transform: uppercase;
    margin: 60px 0 10px;
    font-weight: 300;
}

.size-radio-btn{
    display: inline-block;
    width: 80px;
    height: 80px;
    text-align: center;
    font-size: 20px;
    border: 1px solid #383838;
    border-radius: 50%;
    margin: 10px;
    margin-left: 0;
    line-height: 80px;
    text-transform: uppercase;
    color: #383838;
    cursor: pointer;
}

.size-radio-btn.check{
    background: #383838;
    color: #fff;
}

.btn{
    width: 48%;
    padding: 20px;
    border-radius: 5px;
    background: none;
    border: 1px solid #383838;
    color: #383838;
    font-size: 20px;
    cursor: pointer;
    margin: 20px 0;
    text-transform: capitalize;
}

.cart-btn{
    margin-right: 2%;
    background: #383838;
    color: #fff;
}
<section class="detail-des">
    <h2 class="heading">description</h2>
    <p class="des">Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam, ......</p>
</section>
.detail-des{
    padding: 0 10vw;
    text-transform: capitalize;
}

.heading{
    font-size: 30px;
    margin-bottom: 30px;
}

.des{
    color: #383838;
    line-height: 25px;
}
const productImageSlide = document.querySelector(".image-slider"); // seclecting image slider element

let activeImageSlide = 0; // default slider image

productImages.forEach((item, i) => { // loopinh through each image thumb
    item.addEventListener('click', () => { // adding click event to each image thumbnail
        productImages[activeImageSlide].classList.remove('active'); // removing active class from current image thumb
        item.classList.add('active'); // adding active class to the current or clicked image thumb
        productImageSlide.style.backgroundImage = `url('${item.src}')`; // setting up image slider's background image
        activeImageSlide = i; // updating the image slider variable to track current thumb
    })
})
// toggle size buttons

const sizeBtns = document.querySelectorAll('.size-radio-btn'); // selecting size buttons
let checkedBtn = 0; // current selected button

sizeBtns.forEach((item, i) => { // looping through each button
    item.addEventListener('click', () => { // adding click event to each 
        sizeBtns[checkedBtn].classList.remove('check'); // removing check class from the current button
        item.classList.add('check'); // adding check class to clicked button
        checkedBtn = i; // upading the variable
    })
})
<head>
   <link rel="stylesheet" href="css/home.css">
   <link rel="stylesheet" href="css/search.css">
</head>
<body>
    <nav class="navbar"></nav>
    <footer></footer>

    <script src="js/nav.js"></script>
    <script src="js/footer.js"></script>
</body>
<section class="search-results">
    <h2 class="heading">search results for <span>product</span></h2>
</section>
.search-results{
    width: 100%;
    padding: 60px 0;
}

.heading{
    font-size: 20px;
    text-transform: capitalize;
    font-weight: 400;
    margin-bottom: 40px;
    padding: 0 10vw;
}

.heading span{
    font-weight: 700;
}
.product-container{
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    height: auto;
    grid-row-gap: 40px;
}
<img src="img/404.png" class="four-0-four-image" alt="">
<p class="four-0-four-msg">look like you are lost. Head to beack to our <a href="#">homepage</a></p>
.four-0-four-image{
    display: block;
    margin: 60px auto;
}

.four-0-four-msg{
    text-align: center;
    text-transform: capitalize;
    color: #383838;
}

.four-0-four-msg a{
    color: #383838;
}
