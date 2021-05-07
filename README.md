# UTS_PengolahanCitra
#TeknikInformatikaUPB
#UniversitasPelitaBangsa

% --- Executes on button press in pushbutton1.
function pushbutton1_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
angka1=str2num(get(handles.edit1,'string'));
angka2=str2num(get(handles.edit2,'string'));

operator=get(handles.popupmenu1,'value');
if operator==1
   hasil=angka1+angka2;
elseif operator==2
    hasil=angka1-angka2;
elseif operator==3
    hasil=angka1*angka2;
elseif operator==4
    hasil=angka1/angka2;
elseif operator==5
    hasil=angka1^angka2;
end
hasil=num2str(hasil);
set(handles.edit3,'string',hasil)

![image](https://user-images.githubusercontent.com/77254428/117502524-d43c7d80-afa9-11eb-81bd-d287e21a20d4.png)
