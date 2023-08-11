<template>
    <div>
        <div class="blurr"></div>
        <nav>
            <div class="navbar">
                <div>
                    <img src="../assets/logo1.png" alt="My logo" class="myLogo">
                </div>
                <!-- <div class="links">
                    <a href="">Home</a>
                    <a href="">About</a>
                    <a href="">My Projects</a>
                    <a href="">Recommendations</a>
                    <a href="">Clients</a>
                </div> -->
                <div class="nav-btn closed" @click="open">
                    <button>Kind words</button>
                </div>
                <!-- <div class="menu-btn">
                    <span>Menu</span>
                    <i class="ri-menu-4-line"></i>
                </div> -->
            </div>
        </nav>

        <div class="side-nav">
            <div class="navv">
                <div class="navbar">
                    <div>
                        <img src="../assets/logo1.png" alt="My logo" class="myLogo">
                    </div>
                    <button class="closed" @click="close">
                        <span>Close</span>
                        <i class="ri-close-line"></i>
                    </button>
                </div>
            </div>
            <div class="scrool">
                <div class="side-nav_links">
                    <div class="stacked">
                        <div class="pplug">
                            <p>I had the pleasure of collaborating with Emmanuel on our mobile app's frontend development. His technical proficiency and innovative approach brought our vision to life. Emmanuel delivered a beautifully designed and highly intuitive interface that exceeded our expectations. His ability to balance aesthetics with functionality is truly remarkable. It was a pleasure working with someone so reliable and talented.</p>
                            <p>PowerPlug</p>
                        </div>
                        <div class="ojo">
                            <p>I couldn't ask for a better Front End Developer. Communication was 200% and this went above my expectations. He threw in some additional perks for me. I will definitely be working with him for future projects. Happy and very satisfied customer</p>
                            <p>Faithful Ojo</p>
                        </div>
                    </div>
                    <div class="sibn">
                        <p>Working with Emmanuel was an absolute pleasure. His frontend web development expertise and creative problem-solving skills took our website to the next level. <br><br>

                            He not only implemented a responsive design but also optimized performance, resulting in faster loading times and better user experience.<br><br>

                            His commitment to delivering high-quality work within the agreed timeline and budget was impressive. 
                            I highly recommend Emmanuel for anyone seeking a top-notch frontend developer.
                        </p>
                        <p>King Basco</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'navbar',

        methods: {
            open() {
                document.querySelector(".side-nav").classList.add('show');
                document.querySelector(".navv").style.display = 'block'
                document.querySelector("nav").style.display = 'none'
            },
            close() {
                document.querySelector(".side-nav").classList.remove('show')
                document.querySelector(".navv").style.display = 'none'
                document.querySelector("nav").style.display = 'block'
            }
        }
    }
</script>