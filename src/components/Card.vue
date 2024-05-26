<template>
    <div class="q-pa-md">
      <div class="hot-products">
        <h2 class="hot-product-text">OUR HOT PRODUCTS</h2>
        <div class="hot-product-list">
          <q-card class="my-card" v-for="(product, index) in hotProducts" :key="index">
            <div class="product-wrapper" ref="productWrapper">
              <img :src="product.imageUrl" alt="Hot Product" style="width: 100%; height: 50%;">
              <div class="product-details">
                <p class="product-name">{{ product.name }}</p>
                <p class="product-price">{{ product.price }}</p>
                <button class="buy-now-button" @click="buyNow">Buy Now</button>
              </div>
            </div>
          </q-card>
        </div>
      </div>
      <hr class="hr-line1">
      <div class="footer">
        <p class="footer-text">
          Informasi tentang website:<br>
          website ini hanyalah sebagai tampilan interfacenya saja menu- <br>menu maupun fitur yang ada belum sepenuhnya bisa berfungsi <br>dikarenakan developer masih tahap belajar pada website ini <br>menampilkan interface toko online jam tangan pria. Jika nama dan<br>harga tidak valid harap maklum
        </p>
        <hr class="hr-line">
        <p class="footer2">M.TAUFIK KURRAHMAN_223510370_COPYRIGHT 2024</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        hotProducts: [
          {
            name: 'JAM TANGAN PRIA ROLEX GOLD',
            price: 'Rp 1.000.000.00',
            imageUrl: 'https://id-test-11.slatic.net/p/8/jam-tangan-pria-automatic-cowo-big-size-skeleton-rantai-kombiwhite-4439-26909953-41d66b57e3181824d4836dc2e89b102b.jpg'
          },
          {
            name: 'JAM TANGAN PRIA ELEXANDRE CHRITIE',
            price: 'Rp 500.000.00',
            imageUrl: 'https://s0.bukalapak.com/img/5177993302/w-1000/Jam_Tangan_Keren_Elegant_Pria_Alexandre_Christie_AC_6470_Ful.jpg'
          },
          {
        name: 'JAM TANGAN CASIO ORIGINAL PRIA SILVER',
        price: 'Rp 2.500.000.00',
        imageUrl: 'https://s2.bukalapak.com/img/7163721631/w-1000/Jam_Tangan_Casio_Original_Pria_AQ_S800WD_1E.jpg'
      },
      {
        name: 'JAM TANGAN PRIA CASIO G-SHOCK GPW100',
        price: 'Rp 200.000.00',
        imageUrl: 'https://tse1.mm.bing.net/th?id=OIP.RjE6VE1bRlG2GrxTLPu3RgHaHa&pid=Api&P=0&h=180'
      },
      {
        name: 'JAM TANGAN ANTI AIR  ',
        price: 'Rp 300.000.00',
        imageUrl: 'https://tse1.mm.bing.net/th?id=OIP.vNVrsEWYtbh2hv9SC3cX7AHaH4&pid=Api&P=0&h=180'
      },
      {
        name: 'JAM TANGAN PRIA FOSSIL FS567 ORIGINAL',
        price: 'Rp 540.000.00',
        imageUrl: 'https://id-test-11.slatic.net/p/7318e998cf3fd2be1e54852e44cf6fea.jpg'
      },
      {
        name: 'JAM TANGAN PRIA ANTI AIR ORIGINAL BLACK',
        price: 'Rp 350.000.000',
        imageUrl: 'https://tse4.mm.bing.net/th?id=OIP.ylNpuYAAUJzXMb1WM1azhAHaHa&pid=Api&P=0&h=180'
      },
      {
        name: 'JAM TANGAN ORIGINAL STENLIS BLACK',
        price: 'Rp 650.000.00',
        imageUrl: 'https://s3.bukalapak.com/img/8630623163/w-1000/jam_tangan_pria_casio_g_shock_GWG_1000.jpg'
      },
      {
        name: 'JAM TANGAN PRIA CASIO ORIGINAL 1374L',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://s2.bukalapak.com/img/2655997871/w-1000/Jam_Tangan_Casio_Original_Pria_MTP_1374L_1A.jpg' 
      },
      {
        name: 'JAM TANGAN PRIA SCALED SILVER',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://s4.bukalapak.com/img/950796241/w-1000/145862_05e6ffbe-9db3-11e4-bfea-fedc4908a8c2_scaled.jpg'
      },
      {
        name: 'JAM TANGAN PRIA SPORTY',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://s4.bukalapak.com/img/993838732/w-1000/Jam%20Tangan%20Pria%20Original%20Expedition%20CR7%20Sporty.jpg' 
      },
      {
        name: 'JAM TANGAN PRIA CHORO BLACK',
        price: 'Rp 1.000.000.00',
        imageUrl:'https://s2.bukalapak.com/img/2078264231/w-1000/Jam_Tangan_Pria___Cowok_Seiko_Chrono_Aktif_Rantai_Full_Black.jpg' 
      },
      {
        name: 'JAM TANGAN PRIA ARMY ORIGINAL ',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://4.bp.blogspot.com/-laHv26JoK3E/Vmjze944RDI/AAAAAAAAAsY/ojImhoLemcg/s1600/jam%2Btangan%2Bpria%2Bmurah.jpg'  
      },
      {
        name: 'JAM TANGAN PRIA LEX ORIGINAL',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://2.bp.blogspot.com/_Cc3gulUhlvs/TKv8qVtLMzI/AAAAAAAACdc/djp1pMwHSzA/s1600/jam-tangan-seiko.jpg' 
      },
      {
        name: 'JAM TANGAN PRIA SEIKO G20',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://www.waktushop.com/wp-content/uploads/2020/07/skmei-jam-tangan-digital-pria-1508-black-or-black-4.jpg' 
      },
      {
        name: 'JAM TANGAN SEIKO BLACK T04',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://s3.bukalapak.com/img/3605649094/w-1000/1019464_7d54c534_b402_455a_83c3_953da1b3ab2b_700_700.jpg' 
      },
      {
        name: 'JAM TANGAN PRIA SWISS LEATHER',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://s1.bukalapak.com/img/6164851811/w-1000/Jam_Tangan_Pria_Murah_Swiss_Army_Leather_Edition_Light_Brown.jpg' 
      },
      {
        name: 'JAM TANGAN PRIA  CHORONO GREY',
        price: 'Rp 1.000.000.00',
        imageUrl: 'https://s2.bukalapak.com/img/2078264231/w-1000/Jam_Tangan_Pria___Cowok_Seiko_Chrono_Aktif_Rantai_Full_Black.jpg'  
      },
      {
        name: 'JAM TANGAN PRIA DIESEL ORIGINAL',
        price: 'Rp 6.000.000.00',
        imageUrl: 'https://s2.bukalapak.com/img/2801340031/w-1000/146681_e8105541_6d8b_4199_8e64_2095fa4ee11e.jpg'  
      },

      {
        name: 'JAM TANGAN PRIA CASIO G SHOCK',
        price: 'Rp 1.300.000.00',
        imageUrl: 'https://s0.bukalapak.com/img/577252483/w-1000/Jam_Tangan_Pria_Casio_G_Shock_GA_110TS_8A3_Original.jpg'
      },

      {
        name: 'JAM TANGAN PRIA ROLEX SILVER',
        price: 'Rp 5.000.000.00',
        imageUrl: 'https://s0.bukalapak.com/img/5376322853/w-1000/jam_tangan_rolex_pria.jpg' 
      },

      {
        name: 'JAM TANGAN PRIA KULIT BROWN',
        price: 'Rp 1.250.000.00',
        imageUrl: 'https://s1.bukalapak.com/img/691039667/w-1000/12126298_cf84e41f_7056_4d7b_8e84_581cc10033c4.jpg' 
      },

      {
        name: 'JAM TANGAN LED KOTAK PRIA',
        price: 'Rp 2.000.000.00',
        imageUrl: 'https://cf.shopee.co.id/file/dee43b9db7b6f458b5f917991b589a98' 
      },

      {
        name: 'JAM TANGAN ANTI KARAT  MIRAGE',
        price: 'Rp 1.500.000.00',
        imageUrl: 'https://cf.shopee.co.id/file/88a9abed4f0361f7469cb8fb35c6eb48' 
      },
        ]
      };
    },
    methods: {
      buyNow() {
        console.log('Buy Now button clicked');
      }
    }
  };
  </script>
  
  <style lang="scss" scoped>
  .q-pa-md {
    display: flex;
    flex-direction: column;
    margin: -1px 20px 90px 10px;
  }
  
  .hot-products {
    padding: 20px;
  }
  
  .hot-product-text {
    background-color: rgb(79, 78, 78);
    text-align: center;
    font-size: 24px;
    color: blue;
    border-radius: 10px;
    margin: -350px -30px -300px -20px;
    margin-bottom: 20px;
  }
  
  .hot-product-list {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 20px;
  }
  
  .my-card {
    position: relative;
    width: 100%;
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  }
  
  .product-wrapper {
    position: relative;
    text-align: left;
  }
  
  .product-details {
    padding: 10px;
  }
  
  .product-name {
    font-weight: bold;
    margin-bottom: 5px;
  }
  
  .product-price {
    color: #007bff;
  }
  
  .buy-now-button {
    display: block;
    width: 100%;
    padding: 10px 0;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  
  .buy-now-button:hover {
    background-color: #0056b3;
  }
  
  .footer {
    background-color: transparent;
    color: black;
    padding: 20px;
    border-radius: 10px;
    margin-top: 20px;
    margin-bottom: -200px;
  }
  
  .footer-text {
    text-align: left;
    margin-bottom: 10px;
  }
  
  .footer2 {
    text-align: right;
    margin-top: 20px;
    margin-bottom: -20px;
  }
  
  .hr-line1 {
    border: 1px solid black; 
    margin: -15px 20px; 
  }
  
  .hr-line {
    border-top: 5px solid blue; 
  }
  </style>
  