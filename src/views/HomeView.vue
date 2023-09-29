<template>
  <div id="home">
    <!-- <vedeoPlayer /> -->
    <section id="section1">
      <div id="first_div" class="container">
        <img class="main_bg" src="../assets/images/main_bg2.jpg" alt="" />
        <Header />
        <div class="bottom">
          <div class="left">
            <h1>
              Школа <span>{</span>
              <b>программирования</b>
              <span>}</span> для тех, кому нужны реальные навыки, а не просто
              сертификат
            </h1>
            <hr />
            <p>
              Пройдите тестирование, чтобы получить доступ к бесплатным вводным
              урокам
            </p>
            <RouterLink to="/sign_up" class="start_test_btn"
              >Пройти тестирование</RouterLink
            >
          </div>
          <div class="right">
            <img src="../assets/images/svg_img/Code.svg" />
          </div>
        </div>
        <a @click="myStop()" href="#section2">
          <span ref="span_tag" class="material-symbols-outlined"
            >arrow_downward</span
          >
        </a>
        <img class="line" src="../assets/images/line.svg" alt="" />
      </div>
    </section>
    <div id="bg">
      <section id="section2">
        <div class="container" id="section2_div1">
          <h1>Какие технологии вы изучите:</h1>
          <div class="technology">
            <div class="section2_div1_left">
              <img src="../assets/images/svg_img/photo2.svg" alt="" />
            </div>
            <div class="section2_div1_right">
              <div>
                <li class="python">Язык программирования Python</li>
                <li class="set">Сети</li>
                <li class="data_base">Базы данных</li>
                <li class="flaskAndDjango">Фреймворки Flask и Django</li>
                <li class="test">Отладка и тестирование</li>
                <li class="docker">Docker</li>
                <li class="git">Git</li>
              </div>
              <h2>
                Это необходимый минимум для современного backend-разработчика
              </h2>
            </div>
          </div>
        </div>
        <div class="container" id="section2_div2">
          <h1>Обучение в YtYt – это удобно и результативно</h1>
          <div id="cards">
            <div class="card">
              <img src="../assets/images/svg_img/gobbler1.svg" alt="" />
              <h3>Огромное количество практики</h3>
              <p>
                Более 500 самостоятельных заданий и 20 полноценных больших
                проектов
              </p>
            </div>
            <div class="card">
              <img src="../assets/images/svg_img/gobbler2.svg" alt="" />
              <h3>Современные методики обучения</h3>
              <p>
                Спиральное обучение: погружаемся в материал постепенно, виток за
                витком
              </p>
            </div>
            <div class="card">
              <img src="../assets/images/svg_img/gobbler3.svg" alt="" />
              <h3>Простое и понятное изложение</h3>
              <p>Вместо заумных терминов – примеры из реального мира</p>
            </div>
            <div class="card">
              <img src="../assets/images/svg_img/gobbler4.svg" alt="" />
              <h3>Гибкий график занятий</h3>
              <p>Учитесь в любое время в удобном для вас темпе</p>
            </div>
            <div class="card">
              <img src="../assets/images/svg_img/gobbler5.svg" alt="" />
              <h3>Прямая связь с опытными программистами</h3>
              <p>Задавайте вопросы и отправляйте свой код на проверку</p>
            </div>
            <div class="card">
              <img src="../assets/images/svg_img/gobbler6.svg" alt="" />
              <h3>Оплата небольшими частями</h3>
              <p>
                Платите только за тот материал, который сейчас изучаете, а не за
                весь курс сразу
              </p>
            </div>
            <div class="card">
              <img src="../assets/images/svg_img/gobbler7.svg" alt="" />
              <h3>Быстрый и легкий возврат</h3>
              <p>Если передумаете учиться – вернем деньги за 3 рабочих дня</p>
            </div>
          </div>
        </div>
      </section>
      <section class="container" id="section3">
        <h1>Как происходит обучение на YtYt?</h1>
        <p>
          Обучение должно быть комфортным. Поэтому мы разработали собственную
          платформу для обучения программированию. На ней вы можете не только
          изучать теорию, но и запускать готовые примеры и даже писать свой
          собственный код.
        </p>
        <div id="macbook">
          <img
            class="img_macbook"
            src="../assets/images/png/macbook.png"
            alt=""
          />
          <img
            class="img_content"
            src="../assets/images/svg_img/img_content.svg"
            alt=""
          />
          <div @click="video_play()" class="play">
            <img src="../assets/images/svg_icon/play.svg" alt="" />
          </div>
          <div ref="video_div" @click="video_pause()" id="video_div">
            <!-- <video
              controls
              id="video_tag"
              ref="video_tag"
              src="../assets/video/rolik.mp4"
            ></video> -->
          </div>
        </div>
        <div id="stages">
          <div class="stage_card">
            <h1>01</h1>
            <h3>Весь материал разбит на небольшие уроки</h3>
            <p>
              Теория и практика подаются маленькими порциями. Так вам будет
              легче усваивать новые знания.
            </p>
          </div>
          <div class="hr"></div>
          <div class="stage_card">
            <h1>02</h1>
            <h3>Обучение через практику</h3>
            <p>
              Всё, что вы узнали, вы тут же начинаете применять на практике. Вы
              сразу видите результаты своего труда.
            </p>
          </div>
          <div class="hr"></div>
          <div class="stage_card">
            <h1>03</h1>
            <h3>Нет ограничений по времени</h3>
            <p>
              Можно совмещать учёбу с работой и другими делами. Не нужно
              выпрашивать академический отпуск, если пришлось сделать перерыв.
            </p>
          </div>
        </div>
        <div id="start_course">
          <RouterLink to="/sign_up" class="start_test_btn"
            >Начать обучение<span class="material-symbols-outlined">
              north_east
            </span></RouterLink
          >
          <p>
            Попробуйте, первые уроки бесплатны, но нужно пройти тестирование
          </p>
        </div>
      </section>
    </div>
    <div id="bg2">
      <section id="section4">
        <div class="support container">
          <div class="section4_img">
            <img src="../assets/images/svg_img/photo3.svg" alt="" />
          </div>
          <div class="section4_text">
            <h1>Помощь и поддержка</h1>
            <p>
              Если в процессе обучения возникнут сложности, вы всегда сможете
              задать вопрос своему наставнику.
            </p>
            <p>
              Раз в несколько уроков вы будете получать большое задание, которое
              нужно будет сдавать на проверку код-ревьюеру. Он внимательно
              изучит ваш код, найдет ошибки и поможет вам стать лучше.
            </p>
          </div>
        </div>
        <div class="method container">
          <div class="section4_text">
            <h1>Методика обучения</h1>
            <p>
              Весь учебный материал структурирован по принципу «спирального
              обучения». Сначала вы получаете базовые знания, а затем на каждом
              витке спирали углубляетесь в изученные темы, доводя их понимание
              до совершенства. Такой подход упрощает обучение и гарантирует, что
              вы не пропустите ничего важного.
            </p>
          </div>
          <div class="section4_img">
            <img src="../assets/images/svg_img/photo4.svg" alt="" />
          </div>
        </div>
      </section>
      <section id="section5" class="container">
        <h1>Стоимость обучения</h1>
        <div class="section5div1">
          <div class="section5card">
            <img src="../assets/images/svg_img/oplata_po_etap.svg" alt="" />
            <p>
              Весь курс разбит на несколько блоков. Оплата поэтапная вы платите
              только за тот блок, который сейчас проходите.
            </p>
          </div>
          <div class="section5card">
            <img src="../assets/images/svg_img/publ.svg" alt="" />
            <p>Любой из блоков вы можете оплатить в рассрочку</p>
          </div>
          <div class="section5card">
            <img src="../assets/images/svg_img/vozvrat.svg" alt="" />
            <p>
              Если передумаете учиться, то возврат можно оформить в любой
              момент. Возвращаем деньги за 3 рабочих дня.
            </p>
          </div>
        </div>
        <div class="section5div2">
          <div ref="phoneScrool" class="phone_scrool">
            <img src="../assets/images/svg_icon/phone.svg" alt="" />
            <img src="../assets/images/svg_icon/Arrow_right.svg" alt="" />
          </div>
          <div class="section5div2table">
            <ul>
              <li>Блок</li>
              <li>Стоимость (₽)</li>
              <li>Расчетное время обучения (мес.) *</li>
            </ul>
            <ul>
              <li>Введение в программирование</li>
              <li>Бесплатно</li>
              <li>0.5</li>
            </ul>
            <ul>
              <li>Основы программирования на Python</li>
              <li>9 900</li>
              <li>1</li>
            </ul>
            <ul>
              <li>Python, продвинутый уровень</li>
              <li>14 900</li>
              <li>2.5</li>
            </ul>
            <ul>
              <li>Сети + фреймворк Flask</li>
              <li>14 900</li>
              <li>2.5</li>
            </ul>
            <ul>
              <li>Базы данных</li>
              <li>14 900</li>
              <li>2</li>
            </ul>
            <ul>
              <li>Фреймворк Django</li>
              <li>14 900</li>
              <li>2</li>
            </ul>
            <ul>
              <li>Разработка «боевого» проекта</li>
              <li>9 900</li>
              <li>1.5</li>
            </ul>
            <ul>
              <li>Итого</li>
              <li>79 400</li>
              <li>12</li>
            </ul>
          </div>
        </div>
        <p>* если занятиям уделяется около 20 часов в неделю</p>
        <div class="loudspeak">
          <img src="../assets/images/svg_img/loudspeaker.svg" alt="" />
          <p>
            Все блоки проходятся строго по порядку. Пропустить какой-то блок или
            начать обучение с середины нельзя, даже если вы считаете, что уже
            знаете какую-то часть материала. Только так мы можем гарантировать,
            что вы получите все знания, предусмотренные учебной программой.
          </p>
          <RouterLink to="/sign_up" class="start_test_btn"
            >Начать обучение<span class="material-symbols-outlined">
              north_east
            </span></RouterLink
          >
        </div>
      </section>
      <footer id="footer" class="container">
        <div class="footer_div">
          <div class="logo_and_social">
            <ul class="footer_logo">
              <img src="../assets/images/logo.svg" alt="" />
              <p>Школа программирования</p>
            </ul>
            <ul class="social">
              <a href=""
                ><img src="../assets/images/svg_icon/instagram.svg" alt=""
              /></a>
              <a href="">
                <img src="../assets/images/svg_icon/vkontact.svg" alt="" />
              </a>
              <a href="">
                <img src="../assets/images/svg_icon/facebook.svg" alt=""
              /></a>
              <a href="">
                <img src="../assets/images/svg_icon/youtube.svg" alt="" />
              </a>
            </ul>
          </div>
          <ul class="footer_links">
            <a href="#section2">Чему вы научитесь</a>
            <a href="#section3">Процесс обучения</a>
            <a href="#section5">Стоимость</a>
            <a href="#footer">Контакты</a>
            <RouterLink to="sign_up">Регистрация</RouterLink>
          </ul>
          <div class="contacts">
            <ul>
              <li class="tel">+7 (499) 348 93 96</li>
              <li class="email">info@ytyt.ru</li>
            </ul>
            <ul class="adress">
              <li>ИП Умаров Т. А.</li>
              <li>ИНН 745216229809</li>
              <li>ОГРНИП 315745200001358</li>
            </ul>
          </div>
        </div>
        <hr />
        <ul class="footer_ul">
          <li>© 2022 ytyt — Все права защищены</li>
          <a href="">Пользовательское соглашение</a>
          <a href="">Политика конфиденциальности</a>
        </ul>
      </footer>
    </div>
  </div>
</template>
<script setup>
import { onMounted, onUnmounted, ref } from "vue";
import Header from "../components/Header.vue";
// import vedeoPlayer from "../components/vedeoPlayer.vue";
const span_tag = ref(null);
const myInterval = ref(null);
const myInterval2 = ref(null);
const phoneScrool = ref(null);
const video_tag = ref(null);
const video_div = ref(null);
function myStop() {
  clearInterval(myInterval.value);
}
function myStop2() {
  clearInterval(myInterval2.value);
}
function video_play() {
  video_tag.value.play();
  video_div.value.style.zIndex = "16";
}
function video_pause() {
  if (video_tag.value.play) {
    // video_tag.value.pause();
    video_div.value.style.zIndex = "9";
  }
  // else if (video_tag.value.pause) {
  //   video_tag.value.play();
  // }
}
onMounted(() => {
  myInterval.value = setInterval(function () {
    span_tag.value.classList.toggle("arrow_down");
  }, 1000);
  myInterval2.value = setInterval(function () {
    phoneScrool.value.classList.toggle("phone_scrool_animate");
  }, 700);
});
onUnmounted(() => {
  myStop();
  myStop2();
})();
</script>
<style scoped lang="scss">
#home {
  display: flex;
  flex-direction: column;
  align-items: center;

  #section1 {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #f9f8fd;
    width: 100vw;
    overflow: hidden;
    #first_div {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 20px 10px 30px 10px;
      position: relative;
      gap: 10px;
      @include media("<=1160px") {
        width: 100%;
      }
      &::before {
        content: "";
        position: absolute;
        width: 100%;
        height: 46px;
        bottom: 0;
        left: -99%;
        background-color: #ffffff;
        z-index: 9;
      }
      &::after {
        content: "";
        position: absolute;
        width: 100%;
        height: 46px;
        bottom: 0;
        right: -99%;
        background-color: #ffffff;
        z-index: 9;
      }
      > .main_bg {
        width: 1800px;
        position: absolute;
        right: -679px;
        top: -475px;
        @include media("<=1000px") {
          right: -50%;
          top: -50px;
          // bottom: -550px !important;
          // transform: translate();
          // transform: translate(-70px, -50px);
        }
      }
      .bottom {
        width: 100%;
        display: flex;
        justify-content: space-between;
        @include media("<=1000px") {
          gap: 50px;
          flex-direction: column;
          align-items: center;
        }
        .left {
          padding: 70px 0 100px 0;
          display: flex;
          width: 55%;
          flex-direction: column;
          align-items: flex-start;
          gap: 20px;
          @include media("<=1000px") {
            width: 90%;
            align-items: center;
            text-align: center;
            padding: 25px 0px 35px 0px;
          }
          h1 {
            font-weight: 500;
            font-size: 46px;
            margin-bottom: 25px;
            color: #22253b;
            @include media("<=1000px") {
              font-size: 24px;
            }
            span {
              color: #f15525;
            }
            b {
              font-weight: 700;
            }
          }
          hr {
            width: 55%;
            border: none;
            border-top: 1px solid #dedede;
          }
          p {
            width: 55%;
            font-weight: 400;
            font-size: 16px;
            color: #22253b;
            @include media("<=1000px") {
              font-size: 12px;
            }
          }
        }
        .right {
          img {
            position: relative;
            top: 48px;
            right: 7px;
            @include media("<=1000px") {
              width: 250px;
              top: 0;
              right: 0;
            }
          }
        }
      }
      .line {
        width: 100%;
        position: absolute;
        bottom: 0;
        left: 0;
      }
      > a {
        position: relative;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #ffffff;
        height: 37px;
        width: 37px;
        .arrow_down {
          transition: 0.15s ease-in-out;
          animation: arrow_down_animate 1s linear infinite;
        }
        @keyframes arrow_down_animate {
          0% {
          }
          50% {
            top: 23px;
          }
          100% {
            top: 16px;
          }
        }
        > span {
          position: absolute;
          left: 50%;
          top: 50%;
          transform: translate(-50%, -50%);
          color: #22253b;
          font-weight: 900;
        }
      }
    }
  }
  #bg {
    display: flex;
    flex-direction: column;
    width: 100vw;
    align-items: center;
    background-image: url("../assets/images/main_bg2.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    #section2 {
      display: flex;
      flex-direction: column;
      align-items: center;
      background-color: #ffffff;
      width: 100vw;
      border-radius: 0 0 40px 40px;
      #section2_div1 {
        display: flex;
        flex-direction: column;
        gap: 35px;
        h1 {
          font-weight: 600;
          font-size: 46px;
          text-align: center;
          color: #22253b;
          @include media("<=tablet") {
            font-size: 24px;
          }
        }
        .technology {
          display: grid;
          grid-template-columns: repeat(2, 1fr);
          border-radius: 48px;
          background: #eaf2f5;
          gap: 20px;
          padding: 40px 40px 0 40px;
          @include media("<=tablet") {
            display: flex;
            padding: 17px;
            gap: 0;
          }
          .section2_div1_left {
            display: flex;
            justify-content: center;
            img {
              height: 352;
              width: 407;
              @include media("<=tablet") {
                display: none;
              }
            }
          }
          .section2_div1_right {
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 25px;
            padding-bottom: 25px;
            @include media("<=tablet") {
              padding: 0;
              // justify-content: space-between;
              // align-items: space-berween;
            }
            > div {
              display: flex;
              flex-wrap: wrap;
              gap: 10px;
              @include media("<=tablet") {
                justify-content: space-between;
              }
              @include media("<=645px") {
                justify-content: flex-start;
              }
              @include media("<=560px") {
                justify-content: space-between;
              }

              > li {
                padding: 10px 15px;
                border-radius: 44px;
                font-weight: 400;
                font-size: 17px;
                color: #ffffff;
                text-align: center;
              }
              .python {
                background-color: #5096ff;
                @include media("<=phone") {
                  width: 100%;
                }
              }
              .set {
                background-color: #ffb359;
                @include media("<=phone") {
                  width: 40%;
                }
              }
              .data_base {
                background-color: #ff6f50;
                @include media("<=phone") {
                  width: 55%;
                }
              }
              .flaskAndDjango {
                background-color: #4bd071;
                @include media("<=phone") {
                  width: 100%;
                }
              }
              .test {
                background-color: #50c0ff;
                @include media("<=phone") {
                  width: 100%;
                }
              }
              .docker {
                background-color: #4b77b9;
                @include media("<=phone") {
                  width: 45%;
                }
              }
              .git {
                background-color: #af93ff;
                @include media("<=phone") {
                  width: 45%;
                }
              }
            }
            h2 {
              font-weight: 600;
              font-size: 20px;
              color: #22253b;
              @include media("<=tablet") {
                display: none;
              }
            }
          }
        }
      }
      #section2_div2 {
        display: flex;
        flex-direction: column;
        gap: 35px;
        align-items: center;
        padding: 40px 10px;
        h1 {
          width: 55%;
          text-align: center;
          font-weight: 600;
          font-size: 46px;
          color: #22253b;
          @include media("<=1000px") {
            width: auto;
          }
          @include media("<=tablet") {
            font-size: 24px;
          }
        }
        #cards {
          display: flex;
          justify-content: center;
          flex-flow: wrap;
          gap: 27px;
          .card {
            height: 250px;
            width: 263px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 15px;
            padding: 35px;
            background-color: #eaf2f5;
            border-radius: 30px;
            @include media("<=860px") {
              &:last-child {
                width: 541px;
              }
            }
            @include media("<=600px") {
              width: 145px;
              height: 175px;
              padding: 10px;
              &:last-child {
                width: 145px;
              }
            }
            @include media("<=510px") {
              &:last-child {
                width: 305px;
              }
            }
            @include media("<=340px") {
              &:last-child {
                width: 145px;
              }
            }
            img {
              width: 60px;
              @include media("<=600px") {
                width: 40px;
                height: 40px;
              }
            }
            > h3 {
              font-weight: 600;
              font-size: 16px;
              color: #22253b;
              text-align: center;
              @include media("<=600px") {
                font-size: 12px;
              }
            }
            > p {
              font-weight: 400;
              font-size: 13px;
              color: #22253b;
              text-align: center;
              @include media("<=600px") {
                font-size: 9px;
              }
            }
          }
        }
      }
    }
    #section3 {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 25px;
      padding: 55px 10px 55px 10px;
      overflow: hidden;
      @include media("<=tablet") {
        width: 100%;
      }
      > h1 {
        font-weight: 600;
        font-size: 46px;
        color: #22253b;
        @include media("<=tablet") {
          font-size: 24px;
        }
      }
      > p {
        width: 60%;
        font-weight: 400;
        font-size: 16px;
        color: #22253b;
        text-align: center;
        @include media("<=tablet") {
          font-size: 12px;
        }
      }
      #macbook {
        padding: 15px;
        .img_macbook {
          width: 760px;
          height: 440px;
          -webkit-filter: drop-shadow(0px 50px 100px rgba(25, 26, 38, 0.4));
          filter: drop-shadow(0px 50px 100px rgba(25, 26, 38, 0.4));
          @include media("<=tablet") {
            width: 300px;
            height: 150px;
          }
        }
        .img_content {
          width: 572px;
          height: 355px;
          position: absolute;
          top: 50%;
          left: 50%;
          transform: translate(-50%, calc(-50% - 15px));
          @include media("<=tablet") {
            width: 230px;
            height: 130px;
            transform: translate(-50%, calc(-50% - 5px));
          }
        }
        &::after {
          content: "";
          width: 572px;
          height: 355px;
          position: absolute;
          top: 50%;
          left: 50%;
          transform: translate(-50%, calc(-50% - 15px));
          background-color: rgba(25, 26, 38, 0.76);
          z-index: 9;
          @include media("<=tablet") {
            width: 230px;
            height: 130px;
            transform: translate(-50%, calc(-50% - 5px));
          }
        }
        .play {
          position: absolute;
          width: 80px;
          height: 80px;
          display: flex;
          justify-content: center;
          top: 50%;
          left: 50%;
          transform: translate(-50%, calc(-50% - 15px));
          z-index: 10;
          background-color: #f15525;
          // background-color: black;

          border-radius: 50%;
          @include media("<=tablet") {
            width: 40px;
            height: 40px;
            transform: translate(-50%, calc(-50% - 5px));
          }
          img {
            width: 18px;
            @include media("<=tablet") {
              width: 6px;
            }
          }
          > &::before {
            content: "";
            width: 80px;
            height: 80px;
            position: absolute;
            top: 0;
            left: 0;
            background-color: rgba(241, 85, 37, 0.32);
            z-index: -5;
            border-radius: 50%;
            animation: crescendo 2s linear infinite;
            @include media("<=tablet") {
              width: 40px;
              height: 40px;
            }
          }
          > &::after {
            content: "";
            width: 80px;
            height: 80px;
            position: absolute;
            top: 0;
            left: 0;
            background-color: rgba(241, 85, 37, 0.32);
            z-index: -5;
            border-radius: 50%;
            animation: crescendo 4s linear infinite;
            @include media("<=tablet") {
              width: 40px;
              height: 40px;
            }
          }
          @keyframes crescendo {
            0% {
              transform: scale(0.8);
            }
            50% {
              transform: scale(1.5);
            }
            100% {
              transform: scale(0.8);
            }
          }
        }
        #video_div {
          width: 572px;
          height: 355px;
          position: absolute;
          top: 50%;
          left: 50%;
          transform: translate(-50%, calc(-50% - 15px));
          // z-index: 999;
          #video_tag {
            width: 100%;
            height: 100%;
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            border: 1px solid red;
            background-color: black;
          }
        }
      }
      #stages {
        width: 100%;
        display: flex;
        justify-content: space-between;
        padding: 50px;
        background-color: #ffffff;
        box-shadow: 0px 81px 120px -77px rgba(34, 37, 59, 0.04);
        border-radius: 40px;
        gap: 20px;
        @include media("<=1000px") {
          padding: 20px;
          flex-direction: column;
        }
        .hr {
          height: 250px;
          width: 2px;
          border-right: 1px solid #eaf2f5;
          @include media("<=1000px") {
            height: 2px;
            width: 100%;
            border-bottom: 1px solid #eaf2f5;
          }
        }
        .stage_card {
          width: 285px;
          display: flex;
          flex-direction: column;
          align-items: flex-start;
          @include media("<=1000px") {
            width: auto;
          }
          h1 {
            font-weight: 700;
            font-size: 77px;
            color: #38bff2;
            @include media("<=tablet") {
              font-size: 50px;
            }
          }
          h3 {
            font-weight: 600;
            font-size: 24px;
            color: #22253b;
            @include media("<=tablet") {
              font-size: 20px;
            }
          }
          p {
            text-align: left;
            font-weight: 400;
            font-size: 16px;
            color: #22253b;
            @include media("<=tablet") {
              font-size: 12px;
            }
          }
        }
      }
      #start_course {
        display: flex;
        width: 650px;
        align-items: center;
        gap: 25px;
        padding: 10px 15px;
        background-color: #ffffff;
        border-radius: 110px;

        @include media("<=tablet") {
          width: 100%;
          flex-direction: column;
          gap: 12px;
          border-radius: 30px;
        }
        a {
          width: 50%;
          display: flex;
          align-items: center;
          gap: 10px;
          font-weight: 400;
          font-size: 16px;
          justify-content: center;
          @include media("<=tablet") {
            width: 90%;
          }
          span {
            font-weight: 600;
          }
        }
        p {
          width: 50%;
          font-weight: 600;
          font-size: 15px;
          color: #22253b;
          @include media("<=tablet") {
            width: 80%;
            font-size: 13px;
            text-align: center;
          }
        }
      }
    }
  }
  #bg2 {
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #f9f8fd;
    @include media("<=1160px") {
      align-items: flex-start;
    }
    #section4 {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      border-radius: 80px;
      gap: 30px;
      padding: 90px 0;
      background-color: #ffffff;
      @include media("<=1200px") {
        padding: 50px;
      }

      @include media("<=tablet") {
        padding: 10px;
      }
      .support {
        display: flex;
        gap: 30px;
        @include media("<=1160px") {
          width: 100%;
        }
        @include media("<=tablet") {
          flex-direction: column;
        }
      }
      .method {
        // width: 100%;
        display: flex;
        gap: 30px;
        @include media("<=1160px") {
          width: 100%;
        }
        @include media("<=tablet") {
          flex-direction: column-reverse;
        }
      }
      .section4_img {
        width: 35%;
        padding: 41px 65px;
        border-radius: 40px;
        background-color: #eaf2f5;
        display: flex;
        justify-content: center;
        align-items: center;
        @include media("<=tablet") {
          width: auto;
          padding: 35px 45px;
        }
        img {
          width: 100%;
          @include media("<=tablet") {
            // width: auto;
          }
        }
      }
      .section4_text {
        width: 65%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 18px;
        border-radius: 40px;
        padding: 50px 90px;
        background-color: #eaf2f5;
        @include media("<=tablet") {
          width: auto;
          gap: 15px;
          padding: 30px 20px;
        }
        h1 {
          font-weight: 600;
          font-size: 32px;
          color: #22253b;
        }
        p {
          font-weight: 400;
          font-size: 16px;
          color: #22253b;
        }
      }
    }
    #section5 {
      display: flex;
      flex-direction: column;
      gap: 35px;
      padding: 60px 10px;
      @include media("<=1160px") {
        width: 100%;
      }
      h1 {
        text-align: center;
        color: #22253b;
        font-weight: 600;
        font-size: 46px;
        @include media("<=tablet") {
          font-size: 22px;
        }
      }
      .section5div1 {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 30px;
        @include media("<=tablet") {
          display: flex;
          flex-direction: column;
          align-items: center;
        }
        .section5card {
          display: flex;
          align-items: center;
          gap: 30px;
          @include media("<=tablet") {
            flex-direction: column;
            width: 60%;
          }
          @include media("<=phone") {
            width: 80%;
          }
          img {
            height: 60px;
            @include media("<=phone") {
              width: 50px;
            }
          }
          p {
            font-weight: 400;
            font-size: 16px;
            color: #22253b;
            @include media("<=tablet") {
              text-align: center;
              font-size: 12px;
            }
          }
        }
      }
      .section5div2 {
        overflow-x: scroll;
        .phone_scrool {
          display: none;
          gap: 5px;
          padding: 20px 50px;
          @include media("<=1000px") {
            display: flex;
          }
        }
        .phone_scrool_animate {
          animation: phone_scrool_anim 0.7s linear infinite;
        }
        @keyframes phone_scrool_anim {
          0% {
            transform: translateX(0px);
          }
          50% {
            transform: translateX(25px);
          }
          100% {
            transform: translateX(0);
          }
        }
        .section5div2table {
          width: 1060px;
          display: flex;
          flex-direction: column;
          padding: 40px;
          background-color: #ffffff;
          border-radius: 30px;

          ul {
            display: grid;
            grid-template-columns: repeat(3, 50% 30% 20%);
            padding: 15px 20px;
            border-radius: 10px;
            li {
              font-weight: 400;
              font-size: 20px;
              color: #22253b;
              @include media("<=phone") {
                font-size: 13px;
              }
            }
            &:nth-child(even) {
              background-color: #f3f3f3;
            }
            &:first-child {
              li {
                font-weight: 700;
                font-size: 16px;
                color: #38bff2;
              }
            }
            &:last-child {
              li {
                font-weight: 700;
                font-size: 24px;
                color: #22253b;
                @include media("<=phone") {
                  font-size: 20px;
                }
              }
            }
          }
        }
      }
      > p {
        font-weight: 400;
        font-size: 16px;
        color: #8e8e8e;
        padding: 0 50px;
        @include media("<=phone") {
          // display: none;
          font-size: 12px;
        }
      }
      .loudspeak {
        display: flex;
        align-items: center;
        gap: 30px;
        background-color: #eaf2f5;
        padding: 65px;
        border-radius: 30px;
        @include media("<=tablet") {
          flex-direction: column;
          padding: 25px;
        }
        img {
          width: 90px;
          @include media("<=tablet") {
            width: 75px;
          }
        }
        > p {
          font-weight: 400;
          font-size: 12px;
          color: #22253b;
          @include media("<=tablet") {
            text-align: center;
          }
        }
        a {
          display: flex;
          align-items: center;
          gap: 10px;
          flex-shrink: 0;
        }
      }
    }
    #footer {
      display: flex;
      flex-direction: column;
      gap: 30px;
      @include media("<=1160px") {
        width: 100%;
      }
      .footer_div {
        display: grid;
        grid-template-columns: repeat(3, 60% 20% 20%);
        @include media("<=tablet") {
          display: flex;
          flex-direction: column;
          align-items: center;
          gap: 40px;
        }
        .logo_and_social {
          display: flex;
          flex-direction: column;
          gap: 40px;
          @include media("<=tablet") {
            align-items: center;
          }
          .footer_logo {
            display: flex;
            gap: 20px;
            img {
              width: 90px;
              height: 32px;
            }
            p {
              width: 150px;
              font-weight: 400;
              font-size: 16px;
              color: #8e8e8e;
            }
          }
          .social {
            display: flex;
            gap: 15px;
            a {
              img {
                width: 35px;
              }
            }
          }
        }
        .footer_links {
          display: flex;
          flex-direction: column;
          gap: 25px;
          @include media("<=tablet") {
            text-align: center;
          }
          a {
            font-weight: 400;
            font-size: 13px;
            color: #22253b;
          }
        }
        .contacts {
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          @include media("<=tablet") {
            gap: 40px;
            text-align: center;
          }
          ul {
            .tel {
              font-weight: 400;
              font-size: 16px;
              color: #38bff2;
            }
            .email {
              font-weight: 400;
              font-size: 16px;
              color: #22253b;
            }
          }
          .adress {
            li {
              font-weight: 400;
              font-size: 13px;
              color: #8e8e8e;
            }
          }
        }
      }
      hr {
        border: 1px solid #d8d8d8;
      }
      .footer_ul {
        display: grid;
        grid-template-columns: repeat(3, 55% 22% 23%);
        @include media("<=tablet") {
          display: flex;
          flex-direction: column;
          align-items: center;
          gap: 13px;
        }
        li,
        a {
          font-weight: 400;
          font-size: 16px;
          color: #8e8e8e;
          @include media("<=tablet") {
            font-size: 12px;
          }
        }
        a {
          @include media("<=tablet") {
            color: #f15525;
          }
        }
      }
    }
  }
}
</style>
