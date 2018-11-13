function myFunc(){ 
    var array1,tab,tr,td,tn,row,col; 
    array1=[["Cell1","Cell2"],["Cell3","Cell4"],["Cell5","Cell6"],["Cell7","Cell8"],["Cell9","Cell10"],["Cell11","Cell12"],["Cell13","Cell14"],["Cell15","Cell16"],["Cell17","Cell18"]];//array1[] initialized with array values  
    tab=document.getElementById("dynamic-table"); 
        
    for(row=0;row<array1.length;row++){ 
        tr=document.createElement('tr'); 
            for(col=0;col<array1[row].length;col++){ 
                td=document.createElement('td'); 
                tn=document.createTextNode(array1[row][col]); 
                td.appendChild(tn); 
                tr.appendChild(td); 
            }
                tab.appendChild(tr); 
         }
}
