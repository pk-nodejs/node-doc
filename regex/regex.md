1. With white space chars

   var x = "a b c";
   x.split(/\s+/); // \s for matching white space characters, + for any number of same characters(here white space)
   
2. Match a line on multi line

  var str = `My Contact
             First Name: Pradeep
             Middle Name: Kumar
             Last Name: Tippa
             `;
  var regex = /^Middle Name: ([a-zA-Z ]+)/m;
  var match = str.match(regex);

3. Match with alpha numeric only.
    var str = 'pradeep123';
    var str2 = 'kumar-1_';
    var reg = /^[a-zA-Z0-9]+$/;
    console.log(str.match(reg));
    console.log(str2.match(reg));