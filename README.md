- 👋 Hi, I’m @Rahafcc
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Rahafcc/Rahafcc is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {
if((!textField1.getText().equals("")) && (!jPasswordField1.getText().equals(""))) { String Email = textField1.getText().trim();
String password = jPasswordField1.getText().trim();
if( dataVerification(Email,password) ){
new Home().setVisible(true);
dispose(); }else{
JOptionPane.showMessageDialog(this, "you can't get into your account, email and pass does'nt match ");
} } else {
JOptionPane.showMessageDialog(this, "Please Fill All Fields Correctly"); }
}
  
 
   private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {
boolean isValidFormatT1 = jTextField1.getText().toString().trim().matches("([0-9]{2})/([0-9]{2})/([0-9]{4})"); boolean isValidFormatT2 = jTextField2.getText().toString().trim().matches("([0-9]{2})/([0-9]{2})/([0-9]{4})"); if(!isValidFormatT1)
JOptionPane.showMessageDialog(this, "Please Fill All Field (Start date) Correctly!"); else if(!isValidFormatT2)
JOptionPane.showMessageDialog(this, "Please Fill All Field (End date) Correctly!");
else{
if(jT == null)
new Confirmation().setVisible(true);
 else
new Confirmation(jT).setVisible(true);
dispose(); }
}
  private void jButton7ActionPerformed(java.awt.event.ActionEvent evt) {
if(!CHECK)
JOptionPane.showMessageDialog(this, "Add table information before!"); else{
timer = new Timer(1000, new ActionListener() {
@Override
public void actionPerformed(ActionEvent e) {
SimpleDateFormat sdf = new SimpleDateFormat("
label1.setText(sdf.format(new java.util.Date())); }
HH:mm:ss");
});
timer.start(); }
}
  private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) { // TODO add your handling code here:
if(jT == null)
new Home().setVisible(true);

 
   else
new Home(jT).setVisible(true);
dispose(); }
  private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {
if(jTable.getRowCount()<4){ if(jComboBox2.getSelectedItem().toString().equals("Evening")){
if(iEv <2)
iEv++; else{
JOptionPane.showMessageDialog(this, "No more than two period Evening can be added!");
return; }
} else{
if(iMor <2) iMor++;
else{
JOptionPane.showMessageDialog(this, "No more than two period Morning can be added!");
return; }
}
String[] data = {counter+"", jComboBox1.getSelectedItem().toString(), jComboBox2.getSelectedItem().toString(),
jComboBox3.getSelectedItem().toString(), jComboBox4.getSelectedItem().toString(), (counter)+" AM to "+(counter)+" PM","12","accepted"};
DefaultTableModel tableModel = (DefaultTableModel) jTable.getModel(); tableModel.addRow(data);
counter++;
 } else{
JOptionPane.showMessageDialog(this, "No more than four rows can be added!"); }
}
 private void jButton8ActionPerformed(java.awt.event.ActionEvent evt) { if(label1.getText().toString().equals(" 00:00:00"))
JOptionPane.showMessageDialog(this, "Click on check in before check out!"); else
timer.stop(); }
 
 
   private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) { // TODO add your handling code here:
if(jT == null)
new Home().setVisible(true); else
new Home(jT).setVisible(true); dispose();
}
