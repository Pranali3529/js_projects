const body = document.body;
const tbl = document.createElement("table");
tbl.style.width = '100%';
tbl.setAttribute('border', '1');
const tbody = document.createElement("tbody");

for(let i = 1; i < 11; i++) {
  const tr = tbl.insertRow();
   for( let j = 1; j < 11; j++) {
     const td = tr.insertCell();
     td.appendChild(document.createTextNode(`${i*j}`));
     tr.appendChild(td);
     
   }
  tbody.appendChild(tr);
 
}
tbl.appendChild(tbody);
body.appendChild(tbl);
