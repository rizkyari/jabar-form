<template>
  <div class="hello">
    <h1>Form Pengusulan Penerima Bansos</h1>
    <p>Silahkan isi data dibawah ini dengan benar</p>
    <div class="form-wrapper">
      <form>
        <div class="label">Nama<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan nama anda">
        </div>
        <div class="label">NIK<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="number" placeholder="Masukkan NIK anda">
        </div>
        <div class="label">Nomor Kartu Keluarga<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="number" placeholder="Masukkan nomor kartu keluarga">
        </div>
        <div class="label">Foto KTP<span class="required">*</span></div>
        <div class="control">
          <input class="input-file input" type="file" placeholder="Text input">
        </div>
        <div class="label">Foto Kartu Keluarga<span class="required">*</span></div>
        <div class="control">
          <input  class="input-file input" type="file" placeholder="Text input">
        </div>
        <div class="label">Umur<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="number" placeholder="Masukkan umur anda">
        </div>
        <div class="label">Jenis Kelamin<span class="required">*</span></div>
        <div class="control">
          <label class="form-control">
            <input type="radio" name="gender" />
              Laki - laki
          </label>

          <label class="form-control">
            <input type="radio" name="gender" />
            Perempuan
          </label>
        </div>
        <div class="label">Provinsi<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan provinsi anda">
        </div>
        <div class="label">Kab/Kota<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan kota anda">
        </div>
        <div class="label">Kelurahan/Desa<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan kelurahan anda">
        </div>
        <div class="label">Alamat<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan alamat anda">
        </div>
        <div class="label">RT<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan RT anda">
        </div>
        <div class="label">RW<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan RW anda">
        </div>
        <div class="label">Penghasilan sebelum pandemi<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan penghasilan anda sebelum pandemi">
        </div>
        <div class="label">Penghasilan setelah pandemi<span class="required">*</span></div>
        <div class="control">
          <input v-model="name" class="input" type="text" placeholder="Masukkan penghasilan anda setelah pandemi">
        </div>
        <div class="label">Alasan membutuhkan bantuan<span class="required">*</span></div>
        <div class="control">
          <textarea rows="5" class="reasons" name="reason" placeholder="Masukkan alasan anda"/>
        </div>
        <div>
          <button class="btn-kirim">Kirim</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      name: "",
      email: "",
      gender: "",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.hello{
  padding: 10em 13em;
}

.form-wrapper{
  padding: 3em;
  border-radius: 10px;
  box-shadow: rgba(17, 17, 26, 0.1) 0px 0px 16px;
}

.label{
  text-align: left;
  padding: 0 2% ;
  margin: 1em 0 0 0;
  font-weight: bold;
}

.required{
  color: rgb(243, 85, 85);
}

.input{
  width: 95%;
  padding: 1em;
  border-radius: 5px;
  border: 1px solid black;
  margin: 10px 0;
}

.input-file{
  border: none;
}

.reasons{
  width: 95%;
  border-radius: 5px;
}

.btn-kirim{
  appearance: button;
  backface-visibility: hidden;
  background-color: #405cf5;
  border-radius: 6px;
  border-width: 0;
  box-shadow: rgba(50, 50, 93, .1) 0 0 0 1px inset,rgba(50, 50, 93, .1) 0 2px 5px 0,rgba(0, 0, 0, .07) 0 1px 1px 0;
  box-sizing: border-box;
  color: #fff;
  cursor: pointer;
  font-family: -apple-system,system-ui,"Segoe UI",Roboto,"Helvetica Neue",Ubuntu,sans-serif;
  font-size: 100%;
  height: 44px;
  line-height: 1.15;
  margin: 12px 0 0;
  outline: none;
  overflow: hidden;
  padding: 0 25px;
  position: relative;
  text-align: center;
  text-transform: none;
  transform: translateZ(0);
  transition: all .2s,box-shadow .08s ease-in;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  width: 97%;
}

@media screen and (max-width: 800px) {
  .hello{
    padding: 5em;
  }
}

@media screen and (max-width: 500px) {
  .hello{
    padding: 1em;
  }
}

</style>
