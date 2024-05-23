# meal-maker
codecademy//beginnersjs//practice project
const menu = {
  _menutype: "Italian",
  _menutype: "Indian",
  _menutype: "Mexican",
  _price: 0,

  set meal(mealToCheck) {
    if (typeof mealToCheck === 'string') {
      return this._meal = mealToCheck;
    } else {
      console.log('meal error')
    }
  },

  set price(priceToCheck) {
    if (typeof priceToCheck === 'number') {
      return this._price = priceToCheck;
    } else {
      console.log('price error')
    }
  },

get todaysSpecial() {

if (this._meal && this._price) {

  return `Today's Special is ${this._meal} for $${this._price}!`
} else {

  return `'Meal or price was not set correctly!'`
}

}

};

menu.meal = 'pizza';
menu.price = 8;
console.log(menu.todaysSpecial);
