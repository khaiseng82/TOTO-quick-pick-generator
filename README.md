# TOTO-quick-pick-generator
TOTO quick pick generator
<html>

<head>


<script type="text/javascript">  


var digit1 =0 ;
var digit2 =0 ;
var digit3 =0 ;
var digit4 =0 ;
var digit5 =0 ;
var digit6 =0 ;
var digit7 =0 ;
var toCheck = [];
var sameValue=false;

 function myRandom() {
 
  
 
  var x = Math.floor((Math.random() * 49) + 1);
  
  return x
  
  
} 

function checkNumber(num,arr){

// Get array lenght
var len  = arr.length
// If Number same  == true, no Number same == false
var bools = false;

for(var i =0; i<= len ; i++){

    if( num == arr[i]){
	
	     bools = true;
	
	}
	
	bools= false;
	
	return bools;


}




}     
    
      
  
             
    function calculateOrigin(){
         
                         
        
        
       
        
                   // 1st Digit;
				    digit1 =  myRandom();
					// push value
					
					toCheck.push(digit1);
			
				   
				   // 2nd Digit ;
				     
					
					do{
					
					   digit2 =  myRandom();
					
					
					}while(digit2==digit1);
	
					  
				    //--------------------------------------	 

					  
					  // 3 Digit ;
					  
				    do{
					
					   digit3 =  myRandom();
					
					
					}while(digit3==digit2||digit3==digit1);
	
				
				
					  
					  // 4 Digit ;
					  
					  do{
					
					   digit4 =  myRandom();
					
					
					}while(digit4==digit3||digit4==digit2||digit4==digit1);
					 
			
					  
					   // 5 Digit ;
					   
					   do{
					
					   digit5 =  myRandom();
					
					
					 }while(digit5==digit4||digit5==digit3||digit5==digit2||digit5==digit1);
					  
					   
					   
					
					  
					  // 6 Digit ;
					  
					   do{
					
					   digit6 =  myRandom();
					
					
					 }while(digit6==digit5||digit6==digit4||digit6==digit3||digit6==digit2||digit6==digit1);
					  
					  
					
					  
					  // 7 Digit ;
					  
					   do{
					
					   digit7 =  myRandom();
					
					
					 }while(digit7==digit6||digit7==digit5||digit7==digit4||digit7==digit3||digit7==digit2||digit7==digit1);
					  
					  
					  
					  
					  
					
            
			
	
	

   
               document.getElementById("displayConv").innerHTML =  digit1 +" &nbsp &nbsp "+ digit2  +" &nbsp &nbsp "+digit3 +" &nbsp &nbsp "+digit4 +" &nbsp &nbsp "+digit5 +" &nbsp &nbsp "+digit6;
        
               document.getElementById("displayConv1").innerHTML =  digit7;
    
		   
		   
		   
		   
		   
		   
		   
		   
 
                
            
            
     
            
                
                   
        
  
      }
                    
              
    
    
    
    
    
                
    
    
</script>
    
<header>


<body>
    
    <form class="form-style-9">
        
        <h2></h2>
    <ul>
         <li>
         <label><strong>Toto Number Generator </strong></label>
    
      
        </li>
  
     
      <li>
          
            <input type="button" value="Generate" id="" onclick="calculateOrigin();"/>      
     </li>
        
        <hr>
      <label><b>Your TOTO lucky Number:</b></label><p id="displayConv" ><strong></strong> </p> 
	  <label><b>Additional Number:</b></label> 
	  <p id="displayConv1" ><strong></strong> </p> 
	
   
 
    
     </ul>
    </form>
	
	</body>
	
	</html>
