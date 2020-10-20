<template>
  <div>
    <h3>Sudoku</h3>
    <center>
    <form class="inboard" @submit.prevent="start">
      <table border = "1">
        
         <tr>
            <td><input type="text" id="11" name="11" size="1" v-model.number="makeboard[0][0]"></td>
            <td><input type="text" id="12" name="12" size="1" v-model.number="makeboard[0][1]"></td>
            <td><input type="text" id="13" name="13" size="1" v-model.number="makeboard[0][2]"></td>
            <td><input type="text" id="14" name="14" size="1" v-model.number="makeboard[0][3]"></td>
            <td><input type="text" id="15" name="15" size="1" v-model.number="makeboard[0][4]"></td>
            <td><input type="text" id="16" name="16" size="1" v-model.number="makeboard[0][5]"></td>
            <td><input type="text" id="17" name="17" size="1" v-model.number="makeboard[0][6]"></td>
            <td><input type="text" id="18" name="18" size="1" v-model.number="makeboard[0][7]"></td>
            <td><input type="text" id="19" name="19" size="1" v-model.number="makeboard[0][8]"></td>
         </tr>
         <tr>
            <td><input type="text" id="21" name="21" size="1" v-model.number="makeboard[1][0]"></td>
            <td><input type="text" id="22" name="22" size="1" v-model.number="makeboard[1][1]"></td>
            <td><input type="text" id="23" name="23" size="1" v-model.number="makeboard[1][2]"></td>
            <td><input type="text" id="24" name="24" size="1" v-model.number="makeboard[1][3]"></td>
            <td><input type="text" id="25" name="25" size="1" v-model.number="makeboard[1][4]"></td>
            <td><input type="text" id="26" name="26" size="1" v-model.number="makeboard[1][5]"></td>
            <td><input type="text" id="27" name="27" size="1" v-model.number="makeboard[1][6]"></td>
            <td><input type="text" id="28" name="28" size="1" v-model.number="makeboard[1][7]"></td>
            <td><input type="text" id="29" name="29" size="1" v-model.number="makeboard[1][8]"></td>
         </tr>
         <tr>
            <td><input type="text" id="31" name="31" size="1" v-model.number="makeboard[2][0]"></td>
            <td><input type="text" id="32" name="32" size="1" v-model.number="makeboard[2][1]"></td>
            <td><input type="text" id="33" name="33" size="1" v-model.number="makeboard[2][2]"></td>
            <td><input type="text" id="34" name="34" size="1" v-model.number="makeboard[2][3]"></td>
            <td><input type="text" id="35" name="35" size="1" v-model.number="makeboard[2][4]"></td>
            <td><input type="text" id="36" name="36" size="1" v-model.number="makeboard[2][5]"></td>
            <td><input type="text" id="37" name="37" size="1" v-model.number="makeboard[2][6]"></td>
            <td><input type="text" id="38" name="38" size="1" v-model.number="makeboard[2][7]"></td>
            <td><input type="text" id="39" name="39" size="1" v-model.number="makeboard[2][8]"></td>
         </tr>
         <tr>
            <td><input type="text" id="41" name="41" size="1" v-model.number="makeboard[3][0]"></td>
            <td><input type="text" id="42" name="42" size="1" v-model.number="makeboard[3][1]"></td>
            <td><input type="text" id="43" name="43" size="1" v-model.number="makeboard[3][2]"></td>
            <td><input type="text" id="44" name="44" size="1" v-model.number="makeboard[3][3]"></td>
            <td><input type="text" id="45" name="45" size="1" v-model.number="makeboard[3][4]"></td>
            <td><input type="text" id="46" name="46" size="1" v-model.number="makeboard[3][5]"></td>
            <td><input type="text" id="47" name="47" size="1" v-model.number="makeboard[3][6]"></td>
            <td><input type="text" id="48" name="48" size="1" v-model.number="makeboard[3][7]"></td>
            <td><input type="text" id="49" name="49" size="1" v-model.number="makeboard[3][8]"></td>
         </tr>
         <tr>
            <td><input type="text" id="51" name="51" size="1" v-model.number="makeboard[4][0]"></td>
            <td><input type="text" id="52" name="52" size="1" v-model.number="makeboard[4][1]"></td>
            <td><input type="text" id="53" name="53" size="1" v-model.number="makeboard[4][2]"></td>
            <td><input type="text" id="54" name="54" size="1" v-model.number="makeboard[4][3]"></td>
            <td><input type="text" id="55" name="55" size="1" v-model.number="makeboard[4][4]"></td>
            <td><input type="text" id="56" name="56" size="1" v-model.number="makeboard[4][5]"></td>
            <td><input type="text" id="57" name="57" size="1" v-model.number="makeboard[4][6]"></td>
            <td><input type="text" id="58" name="58" size="1" v-model.number="makeboard[4][7]"></td>
            <td><input type="text" id="59" name="59" size="1" v-model.number="makeboard[4][8]"></td>
         </tr>
         <tr>
            <td><input type="text" id="61" name="61" size="1" v-model.number="makeboard[5][0]"></td>
            <td><input type="text" id="62" name="62" size="1" v-model.number="makeboard[5][1]"></td>
            <td><input type="text" id="63" name="63" size="1" v-model.number="makeboard[5][2]"></td>
            <td><input type="text" id="64" name="64" size="1" v-model.number="makeboard[5][3]"></td>
            <td><input type="text" id="65" name="65" size="1" v-model.number="makeboard[5][4]"></td>
            <td><input type="text" id="66" name="66" size="1" v-model.number="makeboard[5][5]"></td>
            <td><input type="text" id="67" name="67" size="1" v-model.number="makeboard[5][6]"></td>
            <td><input type="text" id="68" name="68" size="1" v-model.number="makeboard[5][7]"></td>
            <td><input type="text" id="69" name="69" size="1" v-model.number="makeboard[5][8]"></td>
         </tr>
         
         <tr>
            <td><input type="text" id="71" name="71" size="1" v-model.number="makeboard[6][0]"></td>
            <td><input type="text" id="72" name="72" size="1" v-model.number="makeboard[6][1]"></td>
            <td><input type="text" id="73" name="73" size="1" v-model.number="makeboard[6][2]"></td>
            <td><input type="text" id="74" name="74" size="1" v-model.number="makeboard[6][3]"></td>
            <td><input type="text" id="75" name="75" size="1" v-model.number="makeboard[6][4]"></td>
            <td><input type="text" id="76" name="76" size="1" v-model.number="makeboard[6][5]"></td>
            <td><input type="text" id="77" name="77" size="1" v-model.number="makeboard[6][6]"></td>
            <td><input type="text" id="78" name="78" size="1" v-model.number="makeboard[6][7]"></td>
            <td><input type="text" id="79" name="79" size="1" v-model.number="makeboard[6][8]"></td>
         </tr>
         <tr>
            <td><input type="text" id="81" name="81" size="1" v-model.number="makeboard[7][0]"></td>
            <td><input type="text" id="82" name="82" size="1" v-model.number="makeboard[7][1]"></td>
            <td><input type="text" id="83" name="83" size="1" v-model.number="makeboard[7][2]"></td>
            <td><input type="text" id="84" name="84" size="1" v-model.number="makeboard[7][3]"></td>
            <td><input type="text" id="85" name="85" size="1" v-model.number="makeboard[7][4]"></td>
            <td><input type="text" id="86" name="86" size="1" v-model.number="makeboard[7][5]"></td>
            <td><input type="text" id="87" name="87" size="1" v-model.number="makeboard[7][6]"></td>
            <td><input type="text" id="88" name="88" size="1" v-model.number="makeboard[7][7]"></td>
            <td><input type="text" id="89" name="89" size="1" v-model.number="makeboard[7][8]"></td>
         </tr>

         <tr>
            <td><input type="text" id="91" name="91" size="1" v-model.number="makeboard[8][0]"></td>
            <td><input type="text" id="92" name="92" size="1" v-model.number="makeboard[8][1]"></td>
            <td><input type="text" id="93" name="93" size="1" v-model.number="makeboard[8][2]"></td>
            <td><input type="text" id="94" name="94" size="1" v-model.number="makeboard[8][3]"></td>
            <td><input type="text" id="95" name="95" size="1" v-model.number="makeboard[8][4]"></td>
            <td><input type="text" id="96" name="96" size="1" v-model.number="makeboard[8][5]"></td>
            <td><input type="text" id="97" name="97" size="1" v-model.number="makeboard[8][6]"></td>
            <td><input type="text" id="98" name="98" size="1" v-model.number="makeboard[8][7]"></td>
            <td><input type="text" id="99" name="99" size="1" v-model.number="makeboard[8][8]"></td>
         </tr>
      </table>
      <button>Submit</button>
   </form>
    </center>
 




  </div>

</template>

<script>

export default {
   
   
  name: 'Sudoku',

  
  data() {
    return{
       setupboard: true,


        makeboard: [[0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0, 0]],



        tt: "hi",
        c: [],
        ss: [], 
        go: [],
        trials: []

        
    }
  },
   watch: {
  
   },
    computed: {
       
   


      

 

  
      
    },
    methods: {
      testing() {
      
      var coor = this.findEmpty() 
      this.isValid(coor, 9)
      
    },
    start() {
       this.solve()
       
    },
    findEmpty() {
      for (var i = 0; i < 9; i++) {
         for (var j = 0; j < 9; j++) {
            if (this.makeboard[i][j] == 0){
               this.c.push([i,j])
               return [i,j]
            }
         }
      }
    },
      isValid(coor, t) {
         this.ss.push(t)
         var k
         for (k = 0; k < 9; k++){
            if (this.makeboard[coor[0]][k] == t){
               this.go.push("no")
               return false
            }

         }
         for (k = 0; k < 9; k++){
            if (this.makeboard[k][coor[1]] == t){
               this.go.push("no")
           
               return false
            }

         }
         var boxi = (coor[0] - (coor[0] % 3)) 
         var boxj = (coor[1] - (coor[1] % 3))

         for (var u = boxi; u < boxi + 3; u++) {
         for (var v = boxj; v < boxj + 3; v++) {
            if (this.makeboard[u][v] == t){
               this.go.push("no")
               
               return false
            }
         }
      }
      this.go.push("yes")
     
      return true

      },
      solve(){
         var coor = this.findEmpty() 
         if(!coor){
            this.tt = "done"
            return true
         }
         for (var s = 1; s < 10; s++){
            
            if(this.isValid(coor, s)){
               this.trials.push("pass")
               
               this.makeboard[coor[0]][coor[1]] = s
               if(this.solve()){
                  return true
               }

               this.makeboard[coor[0]][coor[1]] = 0
            }
            
            

         }
         return false
      },
      
    }


   
      

    }
     
  

  

 
  

</script>