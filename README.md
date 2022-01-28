# roman-convertor
roman number convertor

function convertToRoman(num) {
  let space = "";
  while (num >0){
    if(num>=1000){
      space += "M";
      num -= 1000;
    } else if(num >= 900){
      space += "CM";
      num -= 900;
    } else if( num >= 500){
      space += "D";
      num -= 500;
    } else if( num >= 400){
      space += "CD";
      num -= 400;
    } else if(num >= 100) {
      space += "C";
      num -= 100;   
    } else if(num >= 90){
      space += "XC";
      num -= 90;
    } else if(num >= 50){
      space += "L";
      num -= 50;
    } else if(num >= 40){
      space += "XL";
      num -= 40;
    } else if(num >= 10){
      space += "X";
      num -= 10;
    } else if(num >= 9){
      space += "IX";
      num -= 9;
    } else if(num >= 5){
      space += "V";
      num -= 5;
    } else if(num >= 4){
      space += "IV";
      num -= 4;
    } else if(num >=1){
      space += "I";
      num -= 1;
    }
    else{
      break;
    }
   } 
  return space
}

convertToRoman(36);
console.log(convertToRoman(36))
console.log(convertToRoman(1994))
