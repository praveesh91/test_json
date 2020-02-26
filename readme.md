
POINTS NOTED DURING DEVELOPMENT OF REACT(WILL FORGET) 

In order to execute a function from a child component, you will need to use Refs. React supports a special attribute that you can attach to any component, that's the ref attribute, it takes a callback function, and you can access the functions of the child component in the parent accessing this.refs.REF_NAME.METHOD_NAME.


Context provides a way to pass data through the component tree without having to pass props down manually at every level.ss


API KEY=AIzaSyC8dueIYM2oGRAqzq_M4NfKIUu6gf-WbcE

sudo lsof -i:3000
sudo kill pid
sudo chmod -R 777

Setting state right after click
<Button color="outline-secondary" onClick = {()=> {this.handleLine()}}><i className="fa fa-line-chart"></i></Button>
async handleLine(){
	await this.setState({ chartType:"Line" });
}


Setting state right after changing select
<Input type="select" name="select" id="exampleSelect" onChange={(event)=> {this.handleSelect(event)}}>
	<option value='one'>Parking Sapce A</option>
	<option value='two'>Parking Sapce B</option>
	<option value='three'>Parking Sapce C</option>
	<option value='four'>Parking Sapce D</option>
</Input>
async handleSelect(event){
	await this.setState({dropdownVal: event.target.value})
	console.log("dropdownVal=",this.state.dropdownVal)
}

