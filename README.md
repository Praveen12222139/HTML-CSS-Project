# HTML-CSS-Project
Booking management system using html,css
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="icon" href="icon.jpg">
    <!--<link rel="stlyesheet" href="styles.css">-->
    <title>Movie Booking</title>
    <style>
        .profile-img-box {
    position: relative;
    height: 30px;
    width: 30px;
    border-radius: 50%;
    overflow: hidden;
}
    
        @import url('https://fonts.googleapis.com/css2?family=Joan&display=swap');
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Joan',serif;
}

    
        

.top-bar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.5rem 1rem;
}

        .navigation {
    display: flex;
    list-style:none;
}
   
        .filter,
.cart,
.help,
.menu{
    position: relative;
    width: 20px;
    height:20px;
}
    
        img {
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    object-fit:cover;
}
    
        .left-content,
.right-content{
    display:flex;
    align-items:center;
    text-shadow: 3px 3px rgb(55,0,255);
}
   
    
      .navigation li{
    margin-right: 1rem;
}

  
        a{
    text-decoration: none;
    color: #adadad;
}

   
        .title{
    margin-right: 3rem;
    color:#cd8c38;
    text-shadow: 3px 1px rgb(55,0,255);
}
   
        .active{
    color:#cd8c38;
}
   
        .navigation li a:hover{
    color:#cd8c38;
}
   
        .filter, .menu{
    display: none;
}
   
        .filter,
.cart,
.help{
    margin-right: 1rem;
}
        .filter,
.cart,
.help,
.menu{
    position: relative;
    width: 20px;
    height:20px;
}
   
        body{
    background-color: #1e1f26;
    display: grid;
    grid-template-columns: 1000px;
    justify-content: space-evenly;
}


    
.main-container{
    color:#adadad;
    display: grid;
    grid-template-columns: 1fr 3fr;
    gap: 2rem;
}
   
        
.sidebar{
    background: linear-gradient(45deg,rgba(255,255,255,.05),rgba(205,140,56,.15));
    backdrop-filter: blur(5px);
    height: fit-content;
    border-radius: 1rem;
    padding: 2rem 2.5rem;
}
  
        .sidebar-groups{
    margin-bottom: 1rem;
}
    
.upcoming-img-box{
    position: relative;
    height: 1000px;
    width: 100%;
    border-radius: 1rem;
    overflow: hidden;
    margin-bottom: 1.5rem;
}
  
    .upcoming-title{
        position: absolute;
        top: 2rem;
        left: 2rem;
        color: #cd8c38;
        background-color: #1e1f26;
        padding: .5rem 1rem;
        border-radius: 2rem;
        border: 1px solid #cd8c38;
        font-weight: 500px;
    }
  
    .buttons{
        position: absolute;
        bottom: 2rem;
        left: 2rem;
    }
  
    .btn-alt{
        background-color: #1e1f26;
        color:#cd8c38;
        border: 1px solid #cd8c38;
        margin-left: 1rem;

    }

  
    .btn-alt:hover{
        color: #1e1f26;
        background-color: #cd8c38;
    }
   
        .btn{
    display: inline-block;
    padding: .5rem 1rem;
    background-color: #cd8c38;
    border-radius: 2rem;
    color: #1e1f26;
    transition: .3s;
}
    
        .btn-1{
    width: 100%;
    text-align: center;
}
   
        .btn:hover{
            background-color: #92601f;
        }
    
        .cm-img-box{
    position: relative;
    height: 300px;
    width: auto;
    margin-bottom: 1rem;
    border-radius: .5rem;
    overflow: hidden;
}
   
.current-movies{
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 1.5rem;
}
  
        .current-movie{
    background: linear-gradient(45deg,rgba(255,255,255,0.5),rgba(205,140,56,.15));
    padding: 1rem;
    border-radius: .5rem;
}
   
        .movie-title{
    color:#fff;
    margin-bottom: .2rem;
}
    
        .booking{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 1rem;
}
   
        .movies-container{
    padding-bottom: 2rem;
}
   
        .price{
            color:GOld;
            
        }
   
        .sg-title{
    margin-bottom: .5rem;
    color: #fff;
}
   
        input{
    margin-bottom: .6rem;
}
   
        label{
    margin-left: .5rem;
}
   
          input[type=radio]:checked{
    accent-color: #cd8c38;
}
    
    input[type=checkbox]:checked{
    accent-color: #cd8c38;
    }
    </style> 
</head>
<body>
    <section class="top-bar">
        <div class="left-content">
        <h2 class="title">READY TO WATCH </h2>
        <ul class="navigation">
            <li><a href="index.html">Home</a></li>
            <li><a class="active" href="#">Movies</a></li>
            <li><a href="#">Threaters</a></li>
            <li><a href="#">News</a></li>
        </ul>    
        </div>
        <div class="right-content">
        <img src="filter.png" alt="" class="filter">
        <img src="cart.png" alt="" class="cart">
        <img src="help.png" alt="" class="help">
        <div class="profile-img-box">
            <img src="profile.jpg" alt="">
        </div>
        <img src="D:\movie booking\menu.png" alt="" class="menu">
    </div>
    </section>
    <section class="main-container">
        <div class="sidebar">
            <form action="#">
                <div class="sidebar-groups">
                    <h3 class="sg-title">Categories</h3>
                    <input type="checkbox" id="adventure" name="adventure" value="adventure">
                    <label for="adventure">Adventure</label><br>
                    <input type="checkbox" id="action" name="action" value="action">
                    <label for="action">Action</label><br>
                    <input type="checkbox" id="animation" name="animation" value="animation">
                    <label for="animation">Animation</label><br>
                    <input type="checkbox" id="comedy" name="comedy" value="comedy">
                    <label for="comedy">Comedy</label><br>
                    <input type="checkbox" id="science" name="science" value="science">
                    <label for="science">Science Fiction</label><br>
                    <input type="checkbox" id="thriller" name="thriller" value="thriller">
                    <label for="thriller">Thriller</label><br>
                    <input type="checkbox" id="history" name="history" value="history">
                    <label for="history">History</label><br>
                    <input type="checkbox" id="documentary" name="documentary" value="documentary">
                    <label for="documentary">Documentary</label><br>
                    <input type="checkbox" id="fantasy" name="fantasy" value="fantasy">
                    <label for="fantasy">Fantasy</label><br>
                                 
                </div>
                <div class="sidebar-groups">
                    <h3  class="sg-title">Language</h3>
                    <input type="checkbox" id="english" name="english" value="english">
                    <label for="english">English</label><br>
                    <input type="checkbox" id="hindi" name="hindi" value="hindi">
                    <label for="hindi">Hindi</label><br>

                </div>
                <div class="sidebar-groups">
                    <h3  class="sg-title">Time</h3>  
                    <input type="radio" id="morning" name="time" value="morning">
                    <label for="morning">Morning</label><br>
                    <input type="radio" id="night" name="time" value="night">
                    <label for="night">Night</label><br>


                </div>
                <div class="sidebar-groups">
                    <a href="#" class="btn-1- btn">Apply Filters</a>
                </div>
            </form>
        </div>
        <div class="movies-container">
            <div class="upcoming-img-box">
                <img src="upcoming1.jpg" alt=""> 
                <p class="upcoming-title">Upcoming Movie</p>
                <div class="buttons">
                    <a href="ticket details.html" class="btn">Book Now</a>
                    <a href="upcoming.mp4.mp4" class="btn-alt btn">Play Trailer</a>
                    </div>
                </div>
                
        <div class="current-movies">
            <div class="current-movie">
                <div class="cm-img-box">
                    <img src="movie1.jpg" alt="">
                </div>
                <h3 class="movie-title">Adipurush</h3>
                <p class="screen-name">Screen : Platinum</p>
                <div class="booking">
                    <div class="price">15$</div>
                    <a href="ticket details.html" class="btn">Buy Tickets</a>
                    <a href="movie1.mp4.mp4" class="btn-alt btn">Play Trailer</a>
                </div>
            </div>
            <div class="current-movie">
                <div class="cm-img-box">
                    <img src="movie2.jpg" alt="">
                </div>
                <h3 class="movie-title">Bhediya</h3>
                <p class="screen-name">Screen : Gold</p>
                <div class="booking">
                    <div class="price">12$</div>
                    <a href="ticket details.html" class="btn">Buy Tickets</a>
                    <a href="movie2.mp4.mp4" class="btn-alt btn">Play Trailer</a>
                </div>
            </div>
            <div class="current-movie">
                <div class="cm-img-box">
                    <img src="movie3.jpg" alt="">
                </div>
                <h3 class="movie-title">Freddy</h3>
                <p class="screen-name">Screen : Silver</p>
                <div class="booking">
                    <div class="price">10$</div>
                    <a href="ticket details.html" class="btn">Buy Tickets</a>
                    <a href="movie3.mp4.mp4" class="btn-alt btn">Play Trailer</a>
                </div>
            </div>
        </div>
        </div>
    </section>
    
</body>
</html>
