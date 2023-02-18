<template>
  <div>
    <p
      class="absolute top-[-50px] mb-3 justify-center items-center text-xl text-white bg-red-500 font-serif"
    >
      {{ errorFillForm }}
    </p>

    <div>
      <p class="text-2xl flex justify-center font-serif mb-3">
        Using the below form you can save your data about soil in the database!
      </p>
      <form
        v-on:submit.prevent="submit"
        class="bg-slate-500 grid font-bold w-[1250px] pt-8 pb-8 font-['Open_Sans'] mb-12 border border-2 rounded border-pink-700 flex justify-center item-center shadow-lg shadow-blue-500/50"
      >
        <div class="flex justify-center items-start">
          <div class="mr-8">
            <div class="flex font-bold text-xl pl-3 justify-center">
              <label class="font-bold text-white"
                >Information of data piker</label
              >
            </div>
            <div>
              <div
                class="border rounded border-white bg-slate-400 flex mt-3 mb-3 hover:bg-cyan-600 hover:border-cyan-800"
              >
                <div class="w-24 pl-3 mt-4 font-bold">
                  <label class="font-bold"
                    >Name <strong class="text-red-600">*</strong></label
                  >
                </div>
                <input
                  v-model="form.name"
                  type="text"
                  class="w-96 m-3 rounded pl-3 font-Arial h-8"
                  placeholder="First name and last name"
                />
              </div>

              <div
                class="border rounded border-white bg-slate-400 flex mt-3 mb-3 hover:bg-cyan-600 hover:border-cyan-800"
              >
                <div class="w-24 pl-3 mt-4 font-bold">
                  <label class="font-bold"
                    >Phone <strong class="text-red-600">*</strong></label
                  >
                </div>
                <input
                  v-model="form.phone"
                  type="text"
                  class="w-96 m-3 rounded pl-3 font-Arial h-8"
                  placeholder="Eg. +4900000000"
                />
              </div>

              <div
                class="border rounded border-white bg-slate-400 flex mt-3 mb-3 hover:bg-cyan-600 hover:border-cyan-800"
              >
                <div class="w-24 pl-3 mt-4 font-bold">
                  <label class="font-bold">Email</label>
                </div>
                <input
                  type="text"
                  v-model="form.email"
                  class="w-96 m-3 rounded pl-3 font-Arial h-8"
                  placeholder="Name.Family@hnee.de"
                />
              </div>
            </div>

            <div class="flex font-bold text-xl mt-9 justify-center">
              <label class="font-bold text-white">Location and Date</label>
            </div>

            <div class="">
              <div>
                <div
                  class="border rounded border-white bg-slate-400 flex mt-3 mb-3 hover:bg-cyan-600 hover:border-cyan-800"
                >
                  <div class="w-24 pl-3 mt-4 font-bold">
                    <label class="font-bold"
                      >Place <strong class="text-red-600">*</strong></label
                    >
                  </div>
                  <input
                    v-model="form.place"
                    type="text"
                    class="w-96 m-3 rounded pl-3 font-Arial h-8"
                    placeholder="Name of the city"
                  />
                </div>
                <div
                  class="border rounded border-white bg-slate-400 flex mt-3 mb-3 hover:bg-cyan-600 hover:border-cyan-800"
                >
                  <div class="w-24 pl-3 mt-4 font-bold">
                    <label class="font-bold"
                      >Date <strong class="text-red-600">*</strong></label
                    >
                  </div>
                  <input
                    v-model="form.date"
                    type="datetime-local"
                    class="w-96 m-3 rounded pl-3 font-Arial h-8"
                  />
                </div>
              </div>
            </div>
          </div>
          <div class="ml-8">
            <div class="flex font-bold text-xl mt-3 justify-center">
              <label class="font-bold text-white">
                Percentage of physical composition of soil
              </label>
            </div>

            <div>
              <div
                class="border rounded border-white bg-slate-400 flex mt-3 pl-16 hover:bg-cyan-600 hover:border-cyan-800"
              >
                <div
                  class="w-24 pl-3 mt-4 mb-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4"
                    >Air <strong class="text-red-600">*</strong></label
                  >
                  <input
                    v-model="form.air"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Air"
                  />
                </div>

                <div
                  class="w-24 pl-3 mt-4 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4"
                    >Water <strong class="text-red-600">*</strong></label
                  >
                  <input
                    v-model="form.water"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Water"
                  />
                </div>

                <div
                  class="w-24 pl-3 mt-4 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4"
                    >Minerals<strong class="text-red-600">*</strong></label
                  >
                  <input
                    v-model="form.minerals"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Minerals"
                  />
                </div>

                <div
                  class="w-32 pl-3 mt-4 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4"
                    >Organic <strong class="text-red-600">*</strong></label
                  >
                  <input
                    v-model="form.orgainic"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Organic"
                  />
                </div>
              </div>
            </div>
            <div class="flex font-bold text-xl mt-6 justify-center">
              <label class="font-bold text-white"
                >Percentage of abundant elements in the soils</label
              >
            </div>
            <div>
              <div
                class="border rounded border-white bg-slate-400 flex mt-3 pl-11 pr-11 grid grid-cols-4 max-w-[600px] hover:bg-cyan-600 hover:border-cyan-800"
              >
                <div
                  class="w-24 mt-4 mb-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4">Oxygen</label>
                  <input
                    v-model="form.oxygen"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="O"
                  />
                </div>

                <div
                  class="w-24 pl-3 mt-4 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4">Silicon</label>
                  <input
                    v-model="form.silicon"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Si"
                  />
                </div>

                <div
                  class="w-24 pl-3 mt-4 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-3">Aluminium</label>
                  <input
                    v-model="form.aluminium"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Al"
                  />
                </div>

                <div
                  class="w-32 pl-3 mt-4 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4">Iron </label>
                  <input
                    v-model="form.iron"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Fe"
                  />
                </div>

                <div
                  class="w-24 mt-0 mb-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4">Calcium</label>
                  <input
                    v-model="form.calcium"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Ca"
                  />
                </div>

                <div
                  class="w-24 pl-3 mt-0 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4">Sodium</label>
                  <input
                    v-model="form.sodium"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Na"
                  />
                </div>

                <div
                  class="w-24 pl-3 mt-0 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-3">Potassium</label>
                  <input
                    v-model="form.potassium"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="K"
                  />
                </div>

                <div
                  class="w-32 pl-3 mt-0 ml-3 font-bold inline justify-center items-center"
                >
                  <label class="font-bold pl-4">Magnesium </label>
                  <input
                    v-model="form.magnesium"
                    type="number"
                    min="0"
                    class="w-24 m-1 rounded pl-3 font-Arial h-8"
                    placeholder="Mg"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="flex justify-end absolute top-[430px] left-[640px]">
          <button
            v-on:click="reset"
            class="p-2 w-60 ml-6 mr-3 shadow-lg shadow-yellow-600/20 bg-pink-800 border border-black rounded text-white hover:bg-pink-500 active:bg-yellow-50 active:border-pink-70 active:text-pink-700"
          >
            Reset
          </button>
          <button
            v-on:click="save"
            class="p-2 w-60 ml-3 mr-3 shadow-lg shadow-yellow-600/20 bg-pink-800 border border-black rounded text-white hover:bg-pink-500 active:bg-yellow-50 active:border-pink-70 active:text-pink-700"
          >
            Save
          </button>
        </div>
      </form>
    </div>
    <div
      v-if="popUpSaveData"
      class="fixed top-0 left-0 right-0 bottom-0 w-full h-screen z-50 overflow-hidden bg-gray-700 opacity-90 flex flex-col items-center justify-center"
    >
      <div
        class="flex flex-col justify-first items-center bg-white w-1/4 h-[13rem] border-2 min-w-[400px]"
      >
        <div class="w-full align-center">
          <span class="float-right text-3xl pr-2 text-white cursor-pointer"
            >&times;</span
          >
          <p class="text-center text-xl bg-pink-700 h-8 text-white">
            Attention
          </p>
          <div class="justify-center flex items-center mt-8 mb-8">
            <p>Do you want to submit the informatin?</p>
          </div>
          <div class="flex justify-center gap-5">
            <button
              @click="saveInPopUp"
              class="bg-pink-700 w-24 h-8 border border-pink-900 rounded text-white hover:bg-pink-500 active:bg-yellow-50 active:border-pink-70 active:text-pink-700"
            >
              Yes
            </button>
            <button
              @click="cancelInPopUp"
              class="bg-pink-700 w-24 h-8 border border-pink-900 rounded text-white hover:bg-pink-500 active:bg-yellow-50 active:border-pink-70 active:text-pink-700"
            >
              No
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "ImportData",
  data() {
    return {
      listCityBtn: "Click here to see the cities!",
      listCity: false,
      popUpSaveData: false,
      errorFillForm: "",
      currentCity: null,
      showInfoDatabase: false,
      getFromDatabase: [],
      showInformationBox: true,
      locationDateBox: true,
      PhysicalCompositionBox: true,
      abundantElementsBox: true,
      form: {
        name: "",
        phone: "",
        email: "",
        place: "",
        date: "",
        air: null,
        water: null,
        minerals: null,
        orgainic: null,
        oxygen: null,
        silicon: null,
        aluminium: null,
        iron: null,
        calcium: null,
        sodium: null,
        potassium: null,
        magnesium: null,
      },
      errorMessage: "",

      mycomponents: [
        ["Daily Routine", "Hours per Day"],
        ["Air", 0],
        ["Water", 0],
        ["Minerals", 0],
        ["Orgainic materials", 0],
      ],
      options: {
        width: 1100,
        height: 400,
      },
    };
  },
  methods: {
    reset() {
      if (this.form !== "") {
        (this.form.name = ""),
          (this.form.phone = null),
          (this.form.email = ""),
          (this.form.place = ""),
          (this.form.date = ""),
          (this.form.air = null),
          (this.form.water = null),
          (this.form.minerals = null),
          (this.form.orgainic = null),
          (this.form.oxygen = null),
          (this.form.silicon = null),
          (this.form.aluminium = null),
          (this.form.iron = null),
          (this.form.calcium = null),
          (this.form.sodium = null),
          (this.form.potassium = null),
          (this.form.magnesium = null);
      }
    },
    save() {
      if (
        this.form.name === "" ||
        this.form.phone === null ||
        this.form.place === "" ||
        this.form.date === null ||
        this.form.air === null ||
        this.form.water === null ||
        this.form.minerals === null ||
        this.form.orgainic === null
      ) {
        this.errorFillForm = "Please fill out all the necessary fields!";
        setTimeout(() => {
          this.errorFillForm = "";
        }, 5000);
      } else {
        if (this.popUpSaveData === false) {
          this.popUpSaveData = true;
        }
      }
    },

    saveInPopUp() {
      if (this.popUpSaveData === true) {
        this.popUpSaveData = false;
      }
      axios.post(
        "https://web-database-eb3c0-default-rtdb.firebaseio.com/surveys.json",
        {
          name: this.form.name,
          phone: this.form.phone,
          email: this.form.email,
          place: this.form.place,
          date: this.form.date,
          air: this.form.air,
          water: this.form.water,
          minerals: this.form.minerals,
          orgainic: this.form.orgainic,
          oxygen: this.form.oxygen,
          silicon: this.form.silicon,
          aluminium: this.form.aluminium,
          iron: this.form.iron,
          calcium: this.form.calcium,
          sodium: this.form.sodium,
          potassium: this.form.potassium,
          magnesium: this.form.magnesium,
        }
      );
    },
    cancelInPopUp() {
      if (this.popUpSaveData === true) {
        this.popUpSaveData = false;
      }
    },
  },
};
</script>
