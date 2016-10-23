# jrValidator
jrValidator can be used to validate html forms. it is very simple and light-weight, mainly designed to validate the general html forms with javascript.

#How to use it?
1. download jrValidator src file from github
2. add jrValidator.min.css and jrValidator.min.js to your script
3. now validate your form using the guidelines given below

#How to validate forms?
use jrValidateForm() function:
  jrValidateForm() function will return true if the form is validate or return false and indicate the feilds which are not validate
  ex:
  HTML:
  <form id="form1">
    <!--inputs-->
  </form>
  
  JavaScript:
  $(document).ready(function(){
    //raise an event to validate form by clicking button or anything
    $('some-btn').click(function(){
      if(jrValidateForm('form1')){
        //do your stuff
      }else{
        //handle the invalid form
      }
    });
  });
