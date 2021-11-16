<template>
<!-- 
    -->
    <div style='text-align: center;'><br>
    <h2>Refs</h2>
    <p>You have counted {{this.counter}} times</p>
    <button @click="submit">+1 counter</button>
    
    <button @click="unsubmit">-1 counter</button>
  </div>

    <hello-world/>
     <DxChart
        :data-source="data">
        <DxArgumentAxis :tick-interval="10" />
        <DxSeries type="bar" />
        <DxLegend :visible="false" />
    </DxChart>
    <button
    ref="buttonId"
        @click="sayHelloWorld" style="margin-left: 46.5%; height: 30px;"
    /> 
    <DxButton
    ref="buttonId"
        text="Click me"
         style="margin-left: 46.5%; height: 30px;"
    /> 
</template>
 
<script>
import DxButton from 'devextreme-vue/button';
import HelloWorld from './components/HelloWorld.vue'
import DxChart, {
    DxArgumentAxis,
    DxSeries,
    DxLegend
} from 'devextreme-vue/chart';

const data = [{
    arg: 1990,
    val: 5320816667
}, {
    arg: 2000,
    val: 6127700428
}, {
    arg: 2010,
    val: 6916183482
}]
;
 
export default {
    components: {
        DxButton, 
        DxChart, DxArgumentAxis, DxSeries, DxLegend, HelloWorld
    },

    data() {
        return {
            data, 
            counter: 0
        }
    },
    methods: {
        sayHelloWorld() {
            alert('Hello world!');
            this.$refs.buttonId.innerText = 'Hello Bro';
        },
        submit(){
            if(this.counter == -10){alert('balls')}
      this.counter++;
      console.log(this.$refs)
    },

    unsubmit(){
        if(this.counter == -10){alert('balls')}
        this.counter--

    }
    }
}
</script>