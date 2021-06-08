<template>
  <div>
    <div class="title m-auto mt-3">
      <h2 class="text-center">{{h2}}</h2>
    </div>
    <div class="item">
      <div class="flex justify-end">
        <img class="mb-6rem" :src="`img/${img1}.svg`" alt="" />
      </div>

      <div class="flex items-baseline">
        <div class="number-container">
          <div class="number text-center ml-4rem">1.</div>
        </div>
        <p class="p-1">Erstellen dein Lebenslauf</p>
      </div>
    </div>
  <svg class="-mb-5rem" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
  <path fill="#ffffff" fill-opacity="1" d="M0,160L48,181.3C96,203,192,245,288,250.7C384,256,480,224,576,176C672,128,768,64,864,37.3C960,11,1056,21,1152,58.7C1248,96,1344,160,1392,192L1440,224L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"></path>
</svg>
<div class="item2">
    
    <div class="flex items-baseline">
      <div class="number text-center ml-3rem w-widescreen">2.</div>
      <p class="ml-2">{{p2}}</p>
    </div>
    <div class="flex justify-end">
        <img class="mr-6rem mt-3" :src="`img/${img2}.svg`"  alt="">
    </div>
    <svg class="-mt-2rem" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
  <path fill="#fff" fill-opacity="1" d="M0,224L48,213.3C96,203,192,181,288,192C384,203,480,245,576,266.7C672,288,768,288,864,266.7C960,245,1056,203,1152,181.3C1248,160,1344,160,1392,160L1440,160L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
</svg>
   </div>
    <div class="flex items-center ">
        <div class="number-container">
          <div class="number text-center ml-4rem">3.</div>
        </div>
        <p class="-ml-8" >{{p3}}</p>
      </div> 
      <div class="flex justify-end">
        <img class="mr-6rem -mt-16" :src="`img/${img3}.svg`"  alt="">
    </div>
  </div>
</template>

<script>
export default {
      props: ['h2', 'p1','p2','p3','img1','img2','img3'],

}
</script>

<style scoped>
.title {
  width: 280px;
}
.item {
  margin-right: 19px;
}
img {
  width: 220px;
  height: 145px;
  z-index: 9;
}
.mb-6rem{
      margin-bottom: -6rem;

}
.mr-6rem{
    margin-right: 62px;
}
.-mb-5rem{
    margin-bottom: -5rem;
}
.-mt-2rem{
        margin-top: -2.8rem;
}
.ml-4rem {
  margin-left: 4rem;
}
.ml-3rem {
  margin-left: 35px;
}
h2 {
  letter-spacing: 0px;
  font-size: 25px;
  font-weight: 600;
  color: #4a5568;
}
.number {
  width: 106px;
  height: 156px;
  letter-spacing: 0px;
  font-size: 150px;
  color: #718096;
  z-index: 99;
}
.number-container {
  border-radius: 555rem;
  background: #f7fafc88 0% 0% no-repeat padding-box;
  width: 248px;
  height: 248px;
  margin-left: -4rem;
  flex-shrink: 0;
}
.item2{
    padding-top: 3rem;
    height: 420px;
background: transparent linear-gradient(134deg, #E6FFFA 0%, #EBF4FF 100%) 0% 0% no-repeat padding-box
}
.p-1 {
  width: 100%;
  margin-left: -4rem;
  z-index: 9;
}
p {
  letter-spacing: 0.47px;
  color: #718096;
  font-size: 19px;
}
</style>