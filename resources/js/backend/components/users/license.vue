<template>
    <div>


  <section id="topbar">
        <div class="title">
            <a href="javascript:void(0)" @click="$router.go(-1)" ><i class="fa fa-angle-left"></i></a>
            <p>{{ $t('Company_Profile.value') }}</p>
            <LanguageComponent/>
        </div>
    </section>

    <section class="intro mb-5" >
        <div class="container-fluid">
            <pre>

Totally Foregin Site
Welcome to VNSHOPIE Earn Money

100 Rupees bonus on account.
You can work for free by watching videos.

Minimum deposit is Rs.300
Minimum withdrawal is Rs.200
You will receive the payment within 24 hours.
Bkash, Nagad or rocket.

Working hours:
10 AM TO 12 AM.

Withdrawal Time:
10 AM TO 5PM

The order will reach your wallet within 1-24 hours from the time of payment.

Withdrawal Charge: 5%

We deal directly with YouTube and earn profit from them, so you can earn more by investing here.

You can withdraw your investment money at the end of the term.

You can work with us for 2 years.
thank you.
Expiration date is 10 February 2025
            <img :src="$asseturl+'frontend/img/Task.png?ver=1.0'" style="width:50%" alt="">






            </pre>
        </div>
    </section>




    </div>
</template>
