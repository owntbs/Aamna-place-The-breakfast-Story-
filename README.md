<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Payment - Aamna Place</title>
<style>
body{font-family:Arial;background:#f7f7f7;padding:20px}
.box{max-width:400px;margin:auto;background:#fff;padding:20px;border-radius:10px}
h2{text-align:center}
.qr{width:100%;margin:10px 0}
input,button{width:100%;padding:10px;margin-top:10px}
.confirm{background:green;color:#fff;border:none}
</style>
</head>
<body>

<div class="box">
<h2>💳 Payment</h2>

<label>
<input type="radio" name="pay" checked> Paid via UPI / Paytm
</label>

<img src="upi_qr.png" class="qr" alt="UPI QR">
<img src="paytm_qr.png" class="qr" alt="Paytm QR">

<input type="number" placeholder="Amount (optional)">

<label>📸 Upload Payment Screenshot</label>
<input type="file" accept="image/*">

<button class="confirm" onclick="confirmOrder()">✅ Order Confirmed</button>

<p id="msg" style="text-align:center;font-weight:bold"></p>
</div>

<script>
function confirmOrder(){
document.getElementById("msg").innerText =
"✅ Payment received. Your order is confirmed!";
}
</script>

</body>
</html>
