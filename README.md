# johns-java
Hold my java projects
This was posted at the request of coderanch based on a problem i am having getting the thymeleaf data from my front end back to the controller. the controller looks like this
@RequestMapping(value = "/editpersons", params = "btnSaveEdit", method = RequestMethod.POST)
    public String saveEditPersons(@ModelAttribute ArrayList<Person> personList){
		System.out.println("inside edit code personsList size = " + personList.size());
		for (Person p : personList) {
			System.out.println("person is " + p.getName());
		}
        return "index";
    }
 
 and the sysout size=0
