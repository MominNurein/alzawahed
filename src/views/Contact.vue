<template>
<section class="main-content-section py-5" style="margin-top: 100px;">
  <div class="container">
    <h1 class="text-color">alzawahed Group</h1>
    <div class="row justify-content-center">
      <div class="col-lg-10">
        <div class="card card-body border-0 shadow">
          <div class="row">
            <div class="col-lg-5">
              <div class="card py-5 card-body card-contact bg-theme">
                <h1>Contact Us</h1>
                <!-- ========= 1 ========= -->
                <div class="row align-items-center mb-4">
                  <div class="offset-1 col-6 icon-part me-3">
                  <i class="uil uil-map-marker"></i>
                  </div>
                  <div class="col-6 media-body">
                    <h5 class="mt-0 text-white">Saudi arabia - Riyadh - Alwaha</h5>
                  </div>
                </div>
                <!-- ========= 2 ========= -->
                <div class="row align-items-center mb-4">
                  <div class="offset-1 col-6 icon-part me-3">
                  <i class="uil uil-envelope"></i>
                  </div>
                  <div class="col-6 media-body">
                    <h5 class="mt-0 text-white">info@alzwahed.com</h5>
                  </div>
                </div>
                <!-- ========= 3 ========= -->
                <div class="row align-items-center mb-4">
                  <div class="offset-1 col-6 icon-part me-3">
                  <i class="uil uil-phone"></i>
                  </div>
                  <div class="col-6 media-body">
                    <h5 class="mt-0 text-white">+966112155556 +966112694443 +966114565074 +966112003232</h5>
                  </div>
                </div>
                <!-- ========= end ========= -->
              </div>
            </div>
            <!-- ========= 3 ========= -->
            <div class="col-lg-7">
              <form>
                <div class="form-group">
                  <label for="name">NAME</label>
                  <input type="text" class="form-control" id="name">
                </div>
                <div class="form-group">
                  <label for="phone">PHONE NUMBER</label>
                  <input type="text" class="form-control" id="phone">
                </div>
                <div class="form-group">
                  <label for="email">EMAIL</label>
                  <input type="text" class="form-control" id="email">
                </div>
                <div class="form-group">
                  <label class="mt-2 mb-2" for="checkbox">Service you Intersted with</label>
                  <div class="row">
                    <div class="col-6 mb-2"><MDBCheckbox label="Alzawahed Services & Security Guards" v-model="checkbox1" /></div>
                    <div class="col-6 mb-2"><MDBCheckbox label="Alzawahed IT Solution" v-model="checkbox2" /></div>
                    <div class="col-6 mb-2"><MDBCheckbox label="Alzawahed Freight & logistics" v-model="checkbox3" /></div>
                    <div class="col-6 mb-2"><MDBCheckbox label="Alzawahed Custom Clearance" v-model="checkbox4" /></div>
                    <div class="offset-3 col-6 mb-2"><MDBCheckbox label="Alzawahed General Contracting" v-model="checkbox5" /></div>
                  </div>
                </div>
                <div class="form-group">
                  <label for="message">COMMENT OR MESSAGE</label>
                  <textarea class="form-control" id="message" rows="10"></textarea>
                </div>
                <div class="text-center mt-3">
                  <button type="submit" class="btn btn-success">Submit</button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
</template>

<script>
  import { MDBCheckbox } from "mdb-vue-ui-kit";
  import { ref } from "vue";

  export default {
    name:"Contact",
    components: {
      MDBCheckbox
    },
    setup() {
      const checkbox1 = ref(true);
      const checkbox2 = ref(false);
      const checkbox3 = ref(false);
      const checkbox4 = ref(false);
      const checkbox5 = ref(false);

      return {
        checkbox1,
        checkbox2,
        checkbox3,
        checkbox4,
        checkbox5
      };
    }
  };
</script>

<style scoped>
.bg-theme{
  background: hsl(136, 95%, 30%) !important;
}
.card-contact{
  margin-left: -130px;
}
.card-contact h1{
  color: #fff;
  font-size: 30px;
  position: relative;
  margin-bottom: 40px;
}
.card-contact h1::before{
  content: "";
  height: 3px;
  width: 150px;
  background: #fff;
  position: absolute;
  bottom: -10px;
}
.icon-part{
  height: 50px;
  width: 50px;
  border: 2px solid #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  font-size: 20px;
  border-radius: 50%;
}
</style>