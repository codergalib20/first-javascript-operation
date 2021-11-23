# first-javascript-operation












/*
============================
Solve Problem One
============================
*/
function seerToMon(mon) {
const kg = 40;
const result = mon / kg
if(mon >= 0) {
if (typeof mon == 'number') {
return result
} else {
const warning = 'Weights cannot be made without numbers. Please give number'
return warning
}
} else {
const warnign = 'Please giv me a positive number';
return warnign;
}
}
const addKg = seerToMon(100);
console.log(addKg);
/*
============================
Solve Problem Two
============================
*/
function totalSales(shirt, pant, shoe) {
const shirtPrice = 100;
const pantPrice = 200;
const shoePrice = 500;
if (typeof shirt == 'number' && typeof pant == 'number' && typeof shoe == 'number') {
if(shirt >= 0 && pant >= 0 && shoe >= 0) {
const totalShirtPrice = shirt * shirtPrice;
const totalPantPrice = pant * pantPrice;
const totalShoePrice = shoe * shoePrice;
const totalSalesMony = totalShirtPrice + totalPantPrice + totalShoePrice;
return totalSalesMony
} else {
const warning = 'Price cannot be expressed in negative. Obviously give me three positive number';
return warning;
}
} else {
const warning = 'Money cannot be expressed without number. You give three arguments as number.';
return warning;
}
}
const addQuantity = totalSales(2, 3, 1);
console.log(addQuantity);
/*
============================
Solve Problem Three
============================
*/
function deliveryCost(shirtQuantity) {
const quantityOf100 = 100;
const quantityOf200 = 80;
const quantityUpAll = 50;
if (shirtQuantity >= 0) {
if (typeof shirtQuantity == 'number') {
if (shirtQuantity <= 100) {
const tShirtPrice = shirtQuantity * quantityOf100;
return tShirtPrice;
} else if (shirtQuantity <= 200) {
const dalivery100Quantity = 100 * quantityOf100;
const delivery200Quantity = shirtQuantity - 100;
const delivery100to200Quantity = delivery200Quantity * quantityOf200;
const totalDeliveryCost = dalivery100Quantity + delivery100to200Quantity;
return totalDeliveryCost;
} else {
const dalivery100Quantity = 100 * quantityOf100;
const delivery100to200Quantity = 100 * quantityOf200;
const deliveryUpAllOf200 = shirtQuantity - 200;
const upperAllDeliveryCost = deliveryUpAllOf200 * quantityUpAll;
const totalDeliveryCostInFunction = dalivery100Quantity + delivery100to200Quantity + upperAllDeliveryCost;
return totalDeliveryCostInFunction;
}
} else {
const showErroe = 'Hy I\'m math calculation function please give me only number'
return showErroe
}
} else {
const warning = 'Quantities cannot be expressed with negatives. Give me positive number!'
return warning;
}
}
const totalDeliveryPrice = deliveryCost(230)
console.log(totalDeliveryPrice);
/*
============================
Solve Problem Four
============================
*/
const bestFriendNames1 = ['forhad', 'rifat', 'mazidul', 'kusum', 'joynob', 'diya', 'nazmun'];
function perfectFriend(bestFriendNames) {
let perfectFriendName = '';
for (let i = 0; i < bestFriendNames.length; i++) {
const element = bestFriendNames[i];
if (typeof element == 'string') {
if (element.length == 5) {
perfectFriendName = element
break
} else {
perfectFriendName = 'You don\'t have a friend\'s 5 letter name !!';
}
} else {
const warning = 'Names cannot be expressed without strings. You give the names as strings'
return warning;
}
}
return perfectFriendName
}
const addFrindsName = perfectFriend(bestFriendNames1);
console.log(addFrindsName);
