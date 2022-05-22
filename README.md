Program 1

types array b[1//to 27];
type_i:integer
type_s:string;
tipe_b:boolean;



var S_data:string;
  procedure data_country(s:string;var C1:string;var dd,mm,yy:word);    ////процежкра для определения числа месяца года и формата
  var j,i:intager;r:string;sl:array[1..3] of string[4];
  Begin
  j:=j+1;
  sl:=' ';
  for i:=1 to lenght(S) do begin
    if (S[i]>='0') and (s[i]<='9')//S[i]in['0'...'9']
    then sl[j]:=sl[j]+S[i] else
    begin
      r:=S[i];sl[j]
      j:=j+1;
    end;
    end;
    if lenght(sl[1]=4 then begin    // в каждом таким куче валов делаем проверну всеъ разделителей ./-
      val(s[1],yy,k);
      val(s[2],mm,k);
      val(s[3],dd,k);
      end;
    if r='/' then begin
      if (leght(sl[2])=1) or lenght(sl[3])=1) then country1:='гонконг,тайвань' else
        if (lenght(sl[2])=2) and (lenght(sl[3])=2) amd ((mm<10) or (dd<10)) then 
          country1:='иран,япония' else 
            Country1:='г,т,и,я';
    end;
              if lenght(sl[3]=4 then begin
      val(s[3],yy,k);
      val(s[1],dd,k);
      val(s[2],mm,k);
    end;
    
  end;
  procedure convert_data(dd,mm,yy:word;country2:string;var S_d;string);  //Процедуры для конвертации Прописываем каждые if
  begin
   if (country2='польша') or (country2='Венгрия')//итд 
   then S_d:=srt   ///Не забыть что для каждого месяца может быть ноль в начале,пожтому лучше сделать str_dd,str_mm
    
 
  end;
  
  
  
  
  
  
  
  
  
  
  
  begin
    Writeln('введите дату');readln(S_data);
    Data_country(S_data,country1,d,m,y);
  end.
