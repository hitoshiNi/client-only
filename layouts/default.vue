<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
/*共通設定*/
.main_containts {
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    text-align: center;
    display: block;
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    color: black;
  }

h1{
    font-size: 22px;
    margin-top: 30px;
    margin-bottom: 15px;
  }

h2{
    font-size: 18px;
  }

h3,h4,h5,h6{
    font-size: 14px;
  }

p{
    font-size: 10px;
  }

.button {
    display: block;
    width: 200px;
    padding: 7px 20px;
    border-radius: 25px;
    margin-top: 10px;
    margin-left: auto;
    margin-right: auto;
    text-decoration: none;
    color: #FFF;
    background-color: #4169e1;
    transition: .4s;
  }

.button[disabled]{
  display: block;
  width: 200px;
  padding: 7px 20px;
  border-radius: 25px;
  margin-top: 10px;
  margin-left: auto;
  margin-right: auto;
  text-decoration: none;
  color: #FFF;
  background-color: #BBBBBB;
  transition: .4s;
}
  
.button:hover {
    background-color: #008080;
  }

.button[disabled]:hover{
    display: block;
    width: 200px;
    padding: 7px 20px;
    border-radius: 25px;
    margin-top: 10px;
    margin-left: auto;
    margin-right: auto;
    text-decoration: none;
    color: #FFF;
    background-color: #BBBBBB;
    transition: .4s;
  }

.checkbox{
    font-size: 15px;
    margin-top: 10px;
  }

.footer{
    color: black;
    font-size: 8px;
    margin-top: 15px;
    margin-bottom: 15px;
    margin-left: auto;
    margin-right: auto;
  }



/*top page*/
  
.picture_main_item{
    height: 150px;
    padding: 10px;
    margin-top: 10px;
    border: 1px solid #d3d3d3;
    border-radius:10px ;
  }
.other_items{
   margin-top: 25px;
}
.other_item{
    display: block;
    height: 120px;
    width: 300px;
    border: 1px solid #d3d3d3;
    border-radius: 10px;
    margin-top: 10px;
    margin-left: auto;
    margin-right: auto;
  }


.picture_sub_item{
    height: 90%;
    float: left;
    padding: 5px;
    margin: 5px;
    border: 1px solid #d3d3d3;
    border-radius: 10px;
  }
.picture_sub_item::after{
  content:"";
  display: block;
  clear: both;
}
  
.item_explaine{
    margin-top: 5px;
    margin-right: 80px;
    float: right;
  }

.flow_application{
    margin-top: 25px;
 } 
.step{
  display: block;
  margin-top: 10px;
  margin-right: auto;
  margin-left: auto;
  width: 95%;
  padding: 3px;
  border: 2px solid #d3d3d3;
  background-color: #f5f5f5;
}
.step h3{
  margin-top: 10px;
  margin-bottom: 10px;
  margin-right: auto;
  margin-left: auto;
  width: 80px;
  height: 25px;
  padding: 2px;
  background-color: #4169e1;
  color: white;
}
 .attention{
  margin-top: 25px;
} 

.details_application{
      width: 95%;
      height: 150px;
      overflow: scroll;
      background: #ffffff;
      border: 1px solid #cccccc;
      padding: 10px;
      margin-top: 25px;
      margin-left: auto;
      margin-right: auto;
  }


/*tweet*/

.tweet_outer{
      width: 80%;
      height: 380px;
      border: 3px solid #4169e1;
      border-radius:20px;
      background-color: #d3d3d3;
      position: relative;
      margin-top: 15px;
      margin-left: auto;
      margin-right: auto;
      }
.tweet_inner{
    width: 90%;
    height: 95%;
    border: 0px solid #d3d3d3;
    border-radius:20px;
    background-color: white;
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform : translate(-50%,-50%);
    transform : translate(-50%,-50%);
 }

.tweet_box{
      width: 85%;
      height: 300px;
      background-color: white;
      border: 0px solid;
      margin-left: auto;
      margin-right: auto;
      }

.count_chara{
      font-size: 16px;
      margin-top: 10px;
      margin-right: 10px;
      text-align: right;
  }
      
.popup_window{
    z-index:2;
    width:90%;
    height:90%;
    padding: 1em;
    background:#fff;
  }
.overlay{
    /*　要素を重ねた時の順番　*/
    z-index:1;  
    /*　画面全体を覆う設定　*/
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background-color:rgba(0,0,0,0.5);
    /*　画面の中央に要素を表示させる設定　*/
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
.rule_detail{
      width: 100%;
      height: 500px;
      overflow: scroll;
      background: #ffffff;
      border: 1px solid #cccccc;
      padding: 10px;
  }

  /*応募完了画面*/ 
.done h2{
  margin-top: 10px;
}
.done p{
  margin-top: 10px;
}
.other_campaign{
  display: inline-block;
  height: 100px;
  width:150px;
  border: 3px solid #4169e1;
  margin-top: 5px;
  text-align: center;
  
}

</style>
