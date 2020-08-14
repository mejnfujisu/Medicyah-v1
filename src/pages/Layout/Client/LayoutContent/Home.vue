<template>
  <div class="content background-content-home">
    <!-- <div id="login" class="popup" role="dialog">
      <div class="modal-dialog">
        <div class="story-box">
          <div class="modal-body">
            <button data-dismiss="modal" class="close">&times;</button>
            <h4 class="h4">I am a</h4>
            <form>
              <input class="btn login" type="submit" value="User" />
              <input class="btn login" type="submit" value="Doctor" />
            </form>
          </div>
        </div>
      </div>
    </div> -->
    <!--End Of Login Popup-->

    <div class="main-wrapper">
      <!-- Start Story Area -->
      <section class="story-area-2">
        <div class="container">
          <div class="row align-items-center display-flex">
            <div class="percent-40">
              <div class="banner-content text-center">
                <h1 class="text-white">Diagnosis Service</h1>
                <h4 class="text-white">Making Better Life</h4>
              </div>
            </div>
            <div class="percent-60">
              <div class="story-box">
                <h6 class="text-uppercase">The Symptoms You May Having</h6>
                <ul class="ks-cboxtags">
                  <li>
                    <input type="checkbox" id="checkboxOne" value="Rainbow Dash" />
                    <label for="checkboxOne">Rainbow Dash</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxTwo" value="Cotton Candy" checked />
                    <label for="checkboxTwo">Cotton Candy</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxThree" value="Rarity" checked />
                    <label for="checkboxThree">Rarity</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxFour" value="Moondancer" />
                    <label for="checkboxFour">Moondancer</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxFive" value="Surprise" />
                    <label for="checkboxFive">Surprise</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxSix" value="Twilight Sparkle" checked />
                    <label for="checkboxSix">
                      Twilight
                      Sparkle
                    </label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxSeven" value="Fluttershy" />
                    <label for="checkboxSeven">Fluttershy</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxEight" value="Derpy Hooves" />
                    <label for="checkboxEight">Derpy Hooves</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxNine" value="Princess Celestia" />
                    <label for="checkboxNine">
                      Princess
                      Celestia
                    </label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxTen" value="Gusty" />
                    <label for="checkboxTen">Gusty</label>
                  </li>
                  <li class="ks-selected">
                    <input type="checkbox" id="checkboxEleven" value="Discord" />
                    <label for="checkboxEleven">Discord</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxTwelve" value="Clover" />
                    <label for="checkboxTwelve">Clover</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxThirteen" value="Baby Moondancer" />
                    <label for="checkboxThirteen">
                      Baby
                      Moondancer
                    </label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxFourteen" value="Medley" />
                    <label for="checkboxFourteen">Medley</label>
                  </li>
                  <li>
                    <input type="checkbox" id="checkboxFifteen" value="Firefly" />
                    <label for="checkboxFifteen">Firefly</label>
                  </li>
                </ul>
                <div class="symptom-box-footer-area">
                  <a href="#" class="primary-btn d-inline-flex align-items-center">
                    <span class="mr-10">Next</span>
                    <span class="lnr lnr-arrow-right"></span>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- End Story Area -->

      <!-- Start Footer Widget Area -->
      
      <!-- End Footer Widget Area -->
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      hotelData: [
        {
          id: 1,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        },
        {
          id: 2,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        },
        {
          id: 3,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        },
        {
          id: 4,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        },
        {
          id: 5,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        },
        {
          id: 6,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        },
        {
          id: 7,
          name: "vania",
          description:
            "near vashara bearch, beautiful view sun rise, sun set, free tea at evening",
          phone: "090884121"
        }
      ],
      dailySalesChart: {
        data: {
          labels: ["M", "T", "W", "T", "F", "S", "S"],
          series: [[12, 17, 7, 17, 23, 18, 38]]
        },
        options: {
          lineSmooth: this.$Chartist.Interpolation.cardinal({
            tension: 0
          }),
          low: 0,
          high: 50, // creative tim: we recommend you to set the high sa the biggest value + something for a better look
          chartPadding: {
            top: 0,
            right: 0,
            bottom: 0,
            left: 0
          }
        }
      }
    };
  },
  methods: {
    bookHotel(name) {
      let params = {
        hotelName: name,
        CustomerName: "hey"
      };
      alert(params);
    }
  }
};
</script>
<style>
.md-layout-item.md-size-33 {
  min-width: 50% !important;
  max-width: 50%;
  flex: 0 1 33.3333%;
}
</style>