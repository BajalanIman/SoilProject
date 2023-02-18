<template>
  <div class="w-[1200 px] ">
    <Div
      class="mb-12 font-serif mt-14 flex flex-col justify-center items-center"
    >
      <footer class="flex gap-16">
        <div class="w-96">
          <img
            src="https://d30mzt1bxg5llt.cloudfront.net/public/uploads/images/_signatoryLogo/HNEE_Logo_Engl_gruen.jpg"
            alt=""
          />
        </div>
        <div class="flex flex-col w-96 justify-center items-center">
          <h1 class="text-2xl">Forest Information Technology</h1>
          <p class="text-xl mt-6">Course: Web Databases</p>
          <p class="text-xl mt-6">Student: Iman Bajalan</p>
          <p class="text-xl mt-6">Lecturer: Prof. Dr. Luis Miranda</p>
          <p class="text-l mt-6">January 2023</p>
        </div>

        <div class="w-96">
          <img
            src="http://www.fox-foodprocessinginabox.eu/wp-content/uploads/2019/08/008-sggw.jpg"
            alt=""
          />
        </div>
      </footer>
    </Div>
<!--  -->

    <div class="bg-green-700 w-full h-16 mt-10 mb-15 rounded flex items-center">
      <div>
<a target=”_blank” href="https://esdac.jrc.ec.europa.eu/projects/lucas" class="ml-16 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">ESDAC</a> 
<a target=”_blank” href="https://www.soils.org/membership?gclid=CjwKCAiAuaKfBhBtEiwAht6H78ZYaxexdOc3rwf6jrSACV6T2nCDjYZXy0Rb9HFzLZszLoLLOnguQRoC0OsQAvD_BwE" class="ml-10 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">SSSA</a> 
<a target=”_blank” href="https://solarimpulse.com/land-pollution-solutions?utm_term=soil%20contamination&utm_campaign=Solutions&utm_source=adwords&utm_medium=ppc&hsa_acc=1409680977&hsa_cam=11451944566&hsa_grp=117528790248&hsa_ad=474951699036&hsa_src=g&hsa_tgt=kwd-297353405966&hsa_kw=soil%20contamination&hsa_mt=b&hsa_net=adwords&hsa_ver=3&gclid=CjwKCAiAuaKfBhBtEiwAht6H7yygbL_bavU8S2HiyGz0xdbXlQtw-vZ5hk3L7hTZ8Ma_Dt6i0yfG4BoCaCkQAvD_BwE" class="ml-10 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">Solarimpulse</a> 
</div>
<div class="w-[2px] h-11 ml-16 mr-16 bg-green-900"></div>

<a target=”_blank” href="https://www.hnee.de/en/University/University-for-Sustainable-Development-Eberswalde-E1145.htm" class=" bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">HNEE</a> 
<a target=”_blank” href="https://www.sggw.edu.pl/en/" class="ml-10 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">SGGW</a> 

<div class="w-[2px] h-11 ml-16 mr-16 bg-green-900"></div>

<a target=”_blank” href="https://vuejs.org/" class="bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">Vue</a> 
<a target=”_blank” href="https://tailwindcss.com/" class="ml-10 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">Tailwindcss</a> 
<a target=”_blank” href="https://www.meteomatics.com/en/weather-api/?ppc_keyword=weather%20api&gclid=CjwKCAiAuaKfBhBtEiwAht6H7_3DujhIlvuAlm0_x0Ak9f7O4XjcgRIQ4HTM0IJ4Q0vtaWvgMCwbzBoC14UQAvD_BwE" class="ml-10 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">Meteomatics</a> 
<a target=”_blank” href="https://firebase.google.com/" class="ml-10 bg-green-700 text-white font-bold text-xl hover:text-2xl hover:text-black hover:bg-green-700">Firebase
</a> 
</div>

<p class="mt-12 mb-5 text-justify indent-14 font-serif text-xl">Soils are the most complex and diverse ecosystem in the world. Soils not only provide around 98.8% of the food for humans, but soils also provide a wide range of ecosystem services that meet human needs. </p>
<p class="mb-5 text-justify indent-14 font-serif text-xl">According to a report by <a target=”_blank” href="https://esdac.jrc.ec.europa.eu/projects/lucas">ESDAC</a>, <i> "In 2009, the European Commission extended the periodic Land Use/Land Cover Area Frame Survey (LUCAS) to sample and analyse the main properties of topsoil in 23 Member States of the European Union (EU). This topsoil survey represents the first attempt to build a consistent spatial database of the soil cover across the EU based on standard sampling and analytical procedures, with the analysis of all soil samples being carried out in a single laboratory. Approximately 20,000 points were selected out of the main LUCAS grid for the collection of soil samples."</i> That shows the importance of this subject.</p>
<p class=" mb-5 text-justify indent-14 font-serif text-xl">The present project has been done to create a web application to record the soil texture and the main important minerals in the soil, and also to see the results of other recordings by other people using HTML, CSS, JavaScript, Vue, and firebase.  </p>
    <!--  -->
    <div class="flex flex-col justify-center items-center mt-14 static">
      <div>
      <ImportData>

      </ImportData>
    </div>

    <p class="mb-5 text-justify indent-14 font-serif text-xl">Nowadays, with growing the technology, so many aspects of our daily works are highly depending on databases. For example, banks, online markets, restaurants, mobile service providers, modern greenhouses, scientific publications, and so many other jobs are using databases to deal with customers, users, and employees and their information. data can be easily and quickly stored in a database and then this data can be used in different aspects of work. There are many services we use every day that are powered by databases.</p>
    <p class="mb-5 text-justify indent-14 font-serif text-xl">By clicking on the “database” button all of the datasets recorded in the firebase (our database) will be listed below the button. Then by clicking on each dataset that has been defined by the name of a city as a key of the dataset, some information will appear in a form and shows the information of the sampler as well as the percentage of each element in that specific city.</p>
      <!-- Database -->
      <div class="flex items-start mt-10">
        <div v-if="SoilPhoto">
           <img  class="h-80 w-80" src="../my-project/src/assets/Soil2.png" alt="">
        </div>
        <div class="overflow-auto h-[240px]">
          <button
            @click="callDatabase"
            class="bg-yellow-800 border border-black p-2 w-60 ml-3 mr-3 rounded text-white hover:bg-yellow-600 shadow-lg shadow-yellow-600/20"
          >
            Database
          </button>
          <div v-for="place in getFromDatabase" v-bind:key="place" class="">
            <div class="flex">
              <button
                class="bg-yellow-800 border border-black p-2 w-60 ml-3 mr-3 rounded text-white hover:bg-yellow-600 shadow-lg shadow-yellow-600/20"
                v-on:click="setCurrentCity(place.id)"
              >
                {{ place.place }}
              </button>
            </div>
          </div>
        </div>
        <div class="h-[240px] mb-8 flex font-serif">
          <div
            v-if="currentCity != null"
            class="bg-slate-500 w-[300px] p-2 text-white"
          >
            <h1 class="text-xl pt-2 flex justify-center">Information</h1>
            <div class="flex flex-row mb-3 mt-4">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-4 h-4 mr-2 mt-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z"
                />
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z"
                />
              </svg>
              <P>Location: {{ currentCity[0].place }} </P>
            </div>
            <div class="flex flex-row mb-3">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-4 h-4 mr-2 mt-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"
                />
              </svg>

              <p class="mb-1">Collector: {{ currentCity[0].name }}</p>
            </div>

            <div class="flex flex-row mb-3">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-4 h-4 mr-2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M20.25 3.75v4.5m0-4.5h-4.5m4.5 0l-6 6m3 12c-8.284 0-15-6.716-15-15V4.5A2.25 2.25 0 014.5 2.25h1.372c.516 0 .966.351 1.091.852l1.106 4.423c.11.44-.054.902-.417 1.173l-1.293.97a1.062 1.062 0 00-.38 1.21 12.035 12.035 0 007.143 7.143c.441.162.928-.004 1.21-.38l.97-1.293a1.125 1.125 0 011.173-.417l4.423 1.106c.5.125.852.575.852 1.091V19.5a2.25 2.25 0 01-2.25 2.25h-2.25z"
                />
              </svg>

              <p class="mb-1">Phone: {{ currentCity[0].phone }}</p>
            </div>
            <div class="flex flex-row mb-3">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-4 h-4 mr-2 mt-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75"
                />
              </svg>
              <p>Email: {{ currentCity[0].email }}</p>
            </div>
            <div class="flex flex-row mb-3">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-4 h-4 mr-2 mt-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z"
                />
              </svg>

              <p class="mb-1">Date and time: {{ currentCity[0].date }}</p>
            </div>
          </div>
          <div
            v-if="currentCity != null"
            class="border bg-slate-300 w-[400px] rounded grid grid-cols-3 items-center pl-8"
          >
            <div
              class="border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Oxygen</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].oxygen }}
              </p>
            </div>
            <div
              class="border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Silicon</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].silicon }}
              </p>
            </div>
            <div
              class="border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Aluminium</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].aluminium }}
              </p>
            </div>
            <div
              class="border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Iron</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].iron }}
              </p>
            </div>
            <div
              class="border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Calcium</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].calcium }}
              </p>
            </div>
            <div
              class="border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Sodium</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].sodium }}
              </p>
            </div>
            <div
              class="ml-10 border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Potassium</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].potassium }}
              </p>
            </div>
            <div
              class="ml-10 border border-black w-[90px] h-14 flex flex-col bg-yellow-50 rounded shadow-lg shadow-blue-300/20"
            >
              <div
                class="bg-pink-700 text-white flex justify-center items-center h-7"
              >
                <p>Magnesium</p>
              </div>
              <p class="flex justify-center items-center">
                {{ currentCity[0].magnesium }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div v-if="currentCity != null" class="mt-8 mb-5 flex justify-center items-center font-senfont-serif font-bold text-xl">
    <p>Click the button below to see the location of each sample on the map and pie chart of the physical composition!</p>
  </div>
    <div
      class="mt-8 mb-8 flex justify-center items-center font-senfont-serif font-bold"
    >
    <button
        v-if="currentCity != null"
        @click="showPieChart"
        class="bg-yellow-800 border border-black pl-8 pr-8 pt-2 pb-2 ml-3 mr-3 rounded text-white hover:bg-yellow-600 shadow-lg shadow-yellow-600/20"
      >
        {{ currentCity[0].place }}
      </button>
          </div>

    <!-- map -->
    <div class="flex justify-center items-center font-senfont-serif font-bold">
      <div style="height: 600px; width: 800px">
        <l-map ref="map" v-model:zoom="zoom" :center="[centerA, centerB]">
          <l-tile-layer
            url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png"
            layer-type="base"
            name="OpenStreetMap"
          ></l-tile-layer>
          <l-marker :lat-lng="[centerA, centerB]" clickable: true></l-marker>
        </l-map>
      </div>
    </div>
    <div
      class="mt-8 mb-0 flex justify-center items-center font-senfont-serif font-bold"
      v-if="currentCity != null"
    ></div>
    <GChart type="PieChart" :options="options" :data="mycomponents" />

<div class="absolute button-0 left-[-140px] w-[1500px] h-96 mt-[-30px]" >
  <img class="w-full h-96" src="../my-project/src/assets/Soil-main.jpg" alt="">
</div>
    
  </div>
</template>

<script>
import ImportData from "../src/components/ÎmportData.vue";
import axios from "axios";

import "leaflet/dist/leaflet.css";
import { LMap, LTileLayer, LMarker } from "@vue-leaflet/vue-leaflet";

import { GChart } from "vue-google-charts";
import { Bar } from "vue-chartjs";
import {
  Chart as ChartJS,
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale,
} from "chart.js";

ChartJS.register(

  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale
);

export default {
  components: {
    LMap,
    LMarker,
    LTileLayer,
    ImportData,
    GChart,
    Bar,
  },

  data() {
    return {
      SoilPhoto: true,
      centerA: 42.520008,
      centerB: 13.404954,
      q: "Berlin",
      zoom: 10,
      listCityBtn: "Click here to see the cities!",
      listCity: false,
      currentCity: null,
      showInfoDatabase: false,
      getFromDatabase: [],
      showInformationBox: true,
      locationDateBox: true,
      PhysicalCompositionBox: true,
      abundantElementsBox: true,

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
    showPieChart() {
      axios
        .get(
          "http://api.openweathermap.org/geo/1.0/direct?q=" +
            this.currentCity[0].place +
            "&limit=5&appid=992c20977dbb20bd9b6b36c9a376dc7c",
          null
        )
        .then((response) => {
          this.centerA = response.data[0].lat;
          this.centerB = response.data[0].lon;
          console.log(response.data[0].lat, response.data[0].lon);
        });

      console.log(this.currentCity[0].place);
      this.mycomponents[1][1] = this.currentCity[0].air;
      this.mycomponents[2][1] = this.currentCity[0].water;
      this.mycomponents[3][1] = this.currentCity[0].minerals;
      this.mycomponents[4][1] = this.currentCity[0].orgainic;
    },

    showBarChart() {
      this.chartData.datasets[0].data = [
        this.currentCity[0].oxygen,
        this.currentCity[0].silicon,
        this.currentCity[0].aluminium,
        this.currentCity[0].iron,
        this.currentCity[0].calcium,
        this.currentCity[0].sodium,
        this.currentCity[0].potassium,
        this.currentCity[0].magnesium,
      ];
      console.table(this.chartData.datasets[0].data);
    },

    setCurrentCity(id) {
      this.currentCity = this.getFromDatabase.filter((i) => i.id == id);
      this.SoilPhoto=false;
    },
    showInformation() {
      if (this.showInformationBox === true) {
        this.showInformationBox = false;
      }
    },
    hideInformation() {
      if (this.showInformationBox === false) {
        this.showInformationBox = true;
      }
    },

    showLocationDate() {
      if (this.locationDateBox === true) {
        this.locationDateBox = false;
      }
    },

    hideLocationDate() {
      if (this.locationDateBox === false) {
        this.locationDateBox = true;
      }
    },

    ShowPhysicalCompositio() {
      if (this.PhysicalCompositionBox === true) {
        this.PhysicalCompositionBox = false;
      }
    },

    hidePhysicalCompositio() {
      if (this.PhysicalCompositionBox === false) {
        this.PhysicalCompositionBox = true;
      }
    },

    showAbundantElements() {
      if (this.abundantElementsBox === true) {
        this.abundantElementsBox = false;
      }
    },

    hideAbundantElements() {
      if (this.abundantElementsBox === false) {
        this.abundantElementsBox = true;
      }
    },

    callDatabase() {
      axios
        .get(
          "https://web-database-eb3c0-default-rtdb.firebaseio.com/surveys.json"
        )
        .then((data) => {
          Object.keys(data.data).forEach((i) => {
            data.data[i].id = i;
            this.getFromDatabase.push(data.data[i]);
            console.log(this.getFromDatabase);
          });
        });
    },
    InfoDatabase() {
      if (this.showInfoDatabase === false) {
        this.showInfoDatabase = true;
      }
    },
  },
};
</script>
<style>

</style>