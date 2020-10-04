<template>
  <div>
    <h3>Sudoku</h3>
    <form class="inboard">
      <table border = "1">
        
         <tr>
            <td><input type="text" id="11" name="11" v-model="i11"></td>
            <td><input type="text" id="12" name="12" v-model="i12"></td>
            <td><input type="text" id="13" name="13" v-model="i13"></td>
            <td><input type="text" id="14" name="14" v-model="i14"></td>
            <td><input type="text" id="15" name="15" v-model="i15"></td>
            <td><input type="text" id="16" name="16" v-model="i16"></td>
            <td><input type="text" id="17" name="17" v-model="i17"></td>
            <td><input type="text" id="18" name="18" v-model="i18"></td>
            <td><input type="text" id="19" name="19" v-model="i19"></td>
         </tr>
         <tr>
            <td><input type="text" id="21" name="21" v-model="i21"></td>
            <td><input type="text" id="22" name="22" v-model="i22"></td>
            <td><input type="text" id="23" name="23" v-model="i23"></td>
            <td><input type="text" id="24" name="24" v-model="i24"></td>
            <td><input type="text" id="25" name="25" v-model="i25"></td>
            <td><input type="text" id="26" name="26" v-model="i26"></td>
            <td><input type="text" id="27" name="27" v-model="i27"></td>
            <td><input type="text" id="28" name="28" v-model="i28"></td>
            <td><input type="text" id="29" name="29" v-model="i29"></td>
         </tr>
         <tr>
            <td><input type="text" id="31" name="31" v-model="i31"></td>
            <td><input type="text" id="32" name="32" v-model="i32"></td>
            <td><input type="text" id="33" name="33" v-model="i33"></td>
            <td><input type="text" id="34" name="34" v-model="i34"></td>
            <td><input type="text" id="35" name="35" v-model="i35"></td>
            <td><input type="text" id="36" name="36" v-model="i36"></td>
            <td><input type="text" id="37" name="37" v-model="i37"></td>
            <td><input type="text" id="38" name="38" v-model="i38"></td>
            <td><input type="text" id="39" name="39" v-model="i39"></td>
         </tr>
         <tr>
            <td><input type="text" id="41" name="41" v-model="i41"></td>
            <td><input type="text" id="42" name="42" v-model="i42"></td>
            <td><input type="text" id="43" name="43" v-model="i43"></td>
            <td><input type="text" id="44" name="44" v-model="i44"></td>
            <td><input type="text" id="45" name="45" v-model="i45"></td>
            <td><input type="text" id="46" name="46" v-model="i46"></td>
            <td><input type="text" id="47" name="47" v-model="i47"></td>
            <td><input type="text" id="48" name="48" v-model="i48"></td>
            <td><input type="text" id="49" name="49" v-model="i49"></td>
         </tr>
         <tr>
            <td><input type="text" id="51" name="51" v-model="i51"></td>
            <td><input type="text" id="52" name="52" v-model="i52"></td>
            <td><input type="text" id="53" name="53" v-model="i53"></td>
            <td><input type="text" id="54" name="54" v-model="i54"></td>
            <td><input type="text" id="55" name="55" v-model="i55"></td>
            <td><input type="text" id="56" name="56" v-model="i56"></td>
            <td><input type="text" id="57" name="57" v-model="i57"></td>
            <td><input type="text" id="58" name="58" v-model="i58"></td>
            <td><input type="text" id="59" name="59" v-model="i59"></td>
         </tr>
         <tr>
            <td><input type="text" id="61" name="61" v-model="i61"></td>
            <td><input type="text" id="62" name="62" v-model="i62"></td>
            <td><input type="text" id="63" name="63" v-model="i63"></td>
            <td><input type="text" id="64" name="64" v-model="i64"></td>
            <td><input type="text" id="65" name="65" v-model="i65"></td>
            <td><input type="text" id="66" name="66" v-model="i66"></td>
            <td><input type="text" id="67" name="67" v-model="i67"></td>
            <td><input type="text" id="68" name="68" v-model="i68"></td>
            <td><input type="text" id="69" name="69" v-model="i69"></td>
         </tr>
         <tr>
            <td><input type="text" id="71" name="71" v-model="i71"></td>
            <td><input type="text" id="72" name="72" v-model="i72"></td>
            <td><input type="text" id="73" name="73" v-model="i73"></td>
            <td><input type="text" id="74" name="74" v-model="i74"></td>
            <td><input type="text" id="75" name="75" v-model="i75"></td>
            <td><input type="text" id="76" name="76" v-model="i76"></td>
            <td><input type="text" id="77" name="77" v-model="i77"></td>
            <td><input type="text" id="78" name="78" v-model="i78"></td>
            <td><input type="text" id="79" name="79" v-model="i79"></td>
         </tr>
         <tr>
            <td><input type="text" id="81" name="81" v-model="i81"></td>
            <td><input type="text" id="82" name="82" v-model="i82"></td>
            <td><input type="text" id="83" name="83" v-model="i83"></td>
            <td><input type="text" id="84" name="84" v-model="i84"></td>
            <td><input type="text" id="85" name="85" v-model="i85"></td>
            <td><input type="text" id="86" name="86" v-model="i86"></td>
            <td><input type="text" id="87" name="87" v-model="i87"></td>
            <td><input type="text" id="88" name="88" v-model="i88"></td>
            <td><input type="text" id="89" name="89" v-model="i89"></td>
         </tr>

         <tr>
            <td><input type="text" id="91" name="91" v-model="i91"></td>
            <td><input type="text" id="92" name="92" v-model="i92"></td>
            <td><input type="text" id="93" name="93" v-model="i93"></td>
            <td><input type="text" id="94" name="94" v-model="i94"></td>
            <td><input type="text" id="95" name="95" v-model="i95"></td>
            <td><input type="text" id="96" name="96" v-model="i96"></td>
            <td><input type="text" id="97" name="97" v-model="i97"></td>
            <td><input type="text" id="98" name="98" v-model="i98"></td>
            <td><input type="text" id="99" name="99" v-model="i99"></td>
         </tr>
      </table>
      <button>Submit</button>
   </form>
   {{ makeboard }}



  </div>

</template>

<script>

export default {
   
   
  name: 'Sudoku',

  
  data() {
    return{
        i11: "0",
        i12: "0",
        i13: "0",
        i14: "0",
        i15: "0",
        i16: "0",
        i17: "0",
        i18: "0",
        i19: "0",

        i21: "0",
        i22: "0",
        i23: "0",
        i24: "0",
        i25: "0",
        i26: "0",
        i27: "0",
        i28: "0",
        i29: "0",

        i31: "0",
        i32: "0",
        i33: "0",
        i34: "0",
        i35: "0",
        i36: "0",
        i37: "0",
        i38: "0",
        i39: "0",

        i41: "0",
        i42: "0",
        i43: "0",
        i44: "0",
        i45: "0",
        i46: "0",
        i47: "0",
        i48: "0",
        i49: "0",

        i51: "0",
        i52: "0",
        i53: "0",
        i54: "0",
        i55: "0",
        i56: "0",
        i57: "0",
        i58: "0",
        i59: "0",

        i61: "0",
        i62: "0",
        i63: "0",
        i64: "0",
        i65: "0",
        i66: "0",
        i67: "0",
        i68: "0",
        i69: "0",

        i71: "0",
        i72: "0",
        i73: "0",
        i74: "0",
        i75: "0",
        i76: "0",
        i77: "0",
        i78: "0",
        i79: "0",

        i81: "0",
        i82: "0",
        i83: "0",
        i84: "0",
        i85: "0",
        i86: "0",
        i87: "0",
        i88: "0",
        i89: "0",

        i91: "0",
        i92: "0",
        i93: "0",
        i94: "0",
        i95: "0",
        i96: "0",
        i97: "0",
        i98: "0",
        i99: "0"

        
    }
  },
   watch: {
  
   },
    computed: {
        makeboard() {
            
        return [[Number(this.i11), Number(this.i12), Number(this.i13), Number(this.i14), Number(this.i15), Number(this.i16), Number(this.i17), Number(this.i18), Number(this.i19)],
        [Number(this.i21), Number(this.i22), Number(this.i23), Number(this.i24), Number(this.i25), Number(this.i26), Number(this.i27), Number(this.i28), Number(this.i29)],
        [Number(this.i31), Number(this.i32), Number(this.i33), Number(this.i34), Number(this.i35), Number(this.i36), Number(this.i37), Number(this.i38), Number(this.i39)],
        [Number(this.i41), Number(this.i42), Number(this.i43), Number(this.i44), Number(this.i45), Number(this.i46), Number(this.i47), Number(this.i48), Number(this.i49)],
        [Number(this.i51), Number(this.i52), Number(this.i53), Number(this.i54), Number(this.i55), Number(this.i56), Number(this.i57), Number(this.i58), Number(this.i59)],
        [Number(this.i61), Number(this.i62), Number(this.i63), Number(this.i64), Number(this.i65), Number(this.i66), Number(this.i67), Number(this.i68), Number(this.i69)],
        [Number(this.i71), Number(this.i72), Number(this.i73), Number(this.i74), Number(this.i75), Number(this.i76), Number(this.i77), Number(this.i78), Number(this.i79)],
        [Number(this.i81), Number(this.i82), Number(this.i83), Number(this.i84), Number(this.i85), Number(this.i86), Number(this.i87), Number(this.i88), Number(this.i89)],
        [Number(this.i91), Number(this.i92), Number(this.i93), Number(this.i94), Number(this.i95), Number(this.i96), Number(this.i97), Number(this.i98), Number(this.i99)]
        ]
           },
 

  
      
    },
    methods: {
      testing() {
      
      this.i22 = 19
    },
    findEmpty(makeboard) {
      for (var i = 0; i < 9; i++) {
         for (var j = 0; j < 9; j++) {
            if (makeboard[i][j] == 0){
               return [i,j]
            }
         }
      }
    }
    }


   
      

    }
     
  

  

 
  

</script>