<template>
  <!-- START: RUBY DEMO HEADER -->
  <div class="ruby-menu-demo-header">
    <!-- ########################### -->
    <!-- START: RUBY HORIZONTAL MENU -->
    <div class="ruby-wrapper">
      <button class="c-hamburger c-hamburger--htx visible-xs">
        <span>toggle menu</span>
      </button>
      <ul class="ruby-menu">
        <li class="menu_border">
          <a href="#" class="shop">SHOP BY CATEGORY <i class="fa-solid fa-chevron-down"></i></a>
          <ul class="submenu_width">
            <li class="botton_line" v-for="menu in menus">
              <a href="#">{{ menu.label }}</a>
              <ul class="sec_menu_width">
                <li v-for="sec_level in menu?.second_level">
                  <a href="#">{{ sec_level.label }}</a>
                  <ul>
                    <li class="menu_third" v-for="third_level in sec_level?.third_level">
                      <a href="#">{{ third_level.label }}</a>
                    </li>
                  </ul>
                  <span class="ruby-dropdown-toggle"></span>
                </li>
              </ul>
              <span class="ruby-dropdown-toggle"></span>
            </li>
          </ul>
          <span class="ruby-dropdown-toggle"></span>
        </li>

        <li class="ruby-menu-mega-blog menu_border">
          <a href="#"  class="offertags"><i class="fa-solid fa-tag" style="color: #d8261d; font-size: 30px; "></i> OFFERS</a>
          <span class="ruby-dropdown-toggle"></span>
        </li>
      </ul>
    </div>
    <!-- END:   RUBY HORIZONTAL MENU -->
    <!-- ########################### -->
  </div>
  <!-- END: RUBY DEMO HEADER -->
</template>
<script>
export default {
  name: "App",
  // components: { VueSlickCarousel },
  data() {
    return {
      menus: [
        {
          label: "Fruites & Vegitables",
          second_level: [
            {
              label: "Fresh Vegetables",
              third_level: [
                {
                  label: "Potato, Onion & Tomato",
                },
                {
                  label: "CuCumber & Capsicum",
                },
                {
                  label: "Leafy Vegetables",
                },
                {
                  label: "Root Vegetables",
                },
                {
                  label: "Beans, Brinjals & Okra",
                },
                {
                  label: "Cabbage & Cauliflower",
                },
                {
                  label: "Gourd, Pumpkin, Drumstick",
                },
                {
                  label: "Specialty",
                },
              ],
            },
            {
              label: "Herbs & Seasonings",
              third_level: [],
            },
            {
              label: "Fresh Fruits",
              third_level: [],
            },
            {
              label: "Organic Fruits & Veggies",
              third_level: [],
            },
            {
              label: "Cuts & Sprouts",
              third_level: [],
            },
            {
              label: "Exotic Fruits & Veggies",
              third_level: [],
            },
            {
              label: "Flower Bouquets, Bunches",
              third_level: [],
            },
          ],
        },
        {
          label: "Foodgrains, Oil & Masala",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [],
            },
            {
              label: "Sunglasses",
              third_level: [],
            },
          ],
        },
        {
          label: "Bakery, Cakes & Dairy",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Beverages",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Snacks & Branded Foods",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Beauty & Hygiene",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Cleaning & Household",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Kitchen, Garden & pets",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Eggs, Meat & Fish",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Gourment & World Food",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "Baby Care",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
        {
          label: "View All",
          second_level: [
            {
              label: "Luggage Bags",
              third_level: [
                {
                  label: "Adidas",
                },
                {
                  label: "Burberry",
                },
                {
                  label: "Chloe",
                },
              ],
            },
            {
              label: "Perfumes",
              third_level: [],
            },
            {
              label: "Hand Bags",
              third_level: [
                {
                  label: "Luggage Bags",
                },
                {
                  label: "Luggage Bags",
                },
              ],
            },
            {
              label: "Sunglasses",
              third_level: [
                {
                  label: "Luggage Sunglasses",
                },
                {
                  label: "Luggage Sunglasses",
                },
              ],
            },
          ],
        },
      ],
      
      // settings: {
      //   dots: true,
      //   arrows: true,
      //   focusOnSelect: true,
      //   infinite: true,
      //   speed: 3500,
      //   slidesToShow: 2,
      //   slidesToScroll: 1,
      //   autoplay: true,
      //   lazyLoad: true,
      //   responsive: [
      //     {
      //       breakpoint: 1024,
      //       settings: {
      //         slidesToShow: 3,
      //         slidesToScroll: 3,
      //         infinite: true,
      //         dots: true,
      //       },
      //     },
      //     {
      //       breakpoint: 600,
      //       settings: {
      //         slidesToShow: 2,
      //         slidesToScroll: 2,
      //         initialSlide: 2,
      //         arrows:false,
      //       },
      //     },
      //     {
      //       breakpoint: 480,
      //       settings: {
      //         slidesToShow: 1,
      //         slidesToScroll: 1,
      //         arrows:false
      //       },
      //     },
      //   ],
      // },
    };
  },
};
</script>