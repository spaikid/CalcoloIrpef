/**
 * Calcola il valore IRPEF sulla base delle aliquote 2022
 * Per cambiare la aliquote utilizzate i parametri di fuzione.
 * Le percentuali andranno riportate in valore decimale (23% = 0.23)
 *
 * @param {number} v la base imponibile per il calcolo IRPEF.
 * @param {number} f1 (opzionale) la percentuale della fascia 1.
 * @param {number} f2 (opzionale) la percentuale della fascia 2.
 * @param {number} f3 (opzionale) la percentuale della fascia 3.
 * @param {number} f4 (opzionale) la percentuale della fascia 4.
 * @return Il valore IRPEF.
 * @customfunction
 */
function calcoloIrpef(v = 15000, f1 = 0.23, f2 = 0.25, f3 = 0.35, f4 = 0.43) {
  valore = v;
  if (valore <= 15000){
    out = valore * f1
  }else if (valore > 15000 && valore <= 28000){
    out = 3450 + (valore-15000) * f2
  }else if  (valore > 28000 && valore <= 50000){
    out = 3450 + 3250 + (valore - 28000) * f3
  }else if (valore > 50000){
    out = 3450 + 3250 + 7700 + (valore - 50000) * f4
  }
  //Logger.log(out)
  return(out)
}
