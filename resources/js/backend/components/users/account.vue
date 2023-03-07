<template>
    <div>










           <div data-v-7b9eb5e9="">
                            <div data-v-7b9eb5e9="" class="container justify-content-center align-items-center" style="margin-top: 2.3rem;">
                                <div data-v-7b9eb5e9="" class="card" style="display: inline;">





                                    <div data-v-7b9eb5e9="" class="user text-center">
                                        <div data-v-7b9eb5e9="" class="" style="display: flex;align-items: center;">

                                            <img data-v-7b9eb5e9="" src="https://cdn.pixabay.com/photo/2013/07/13/10/07/man-156584__340.png"  style="border: 1px solid #00000040;
    width: 75px;
    height: 75px;
    margin-right: 10px;
    padding: 3px;" class="rounded-circle" />
                                            <div class="userinfo">
                                                <h4 data-v-7b9eb5e9="" class="mb-0">{{ row.user.name }}</h4>
                                                <span data-v-7b9eb5e9="" class="text-muted d-block mb-2">{{ row.user.mobile }}</span>
                                            </div>

                                        </div>
                                        <button data-v-7b9eb5e9="" class="btn bg-c-lite-green btn-sm btn-shape follow inviteButton" style="border-radius: 0px 40px;">Invitation Code: {{ row.user.username }}</button>
                                    </div>


                                </div>
                            </div>
                            <div data-v-7b9eb5e9="" class="container mb-5">
                                <div data-v-7b9eb5e9="" class="row" style="width: 100%; margin-left: 0%;">
                                    <div data-v-7b9eb5e9="" class="shortcut mb-3 text-center" style="border-left: 2px solid rgb(243, 243, 243);    width: 50% !important;">
                                        <img data-v-7b9eb5e9="" src="https://freepngimg.com/thumb/money/49292-1-wealth-image-png-free-photo-thumb.png" width="25px" />
                                        <div data-v-7b9eb5e9="" class="icon_title">Balance</div>
                                        <div data-v-7b9eb5e9="" class="icon-ammount">
                                            BDT {{ parseFloat(row.user.balance).toFixed(2) }}
                                        </div>
                                    </div>
                                    <div data-v-7b9eb5e9="" class="shortcut mb-3 text-center" style="width: 50% !important;">
                                        <img data-v-7b9eb5e9="" src="https://cdn-icons-png.flaticon.com/512/5501/5501360.png" width="25px" />
                                        <div data-v-7b9eb5e9="" class="icon_title">Today Earnig</div>
                                        <div data-v-7b9eb5e9="" class="icon-ammount">
                                            BDT {{ parseFloat(row.taskearn).toFixed(2) }}
                                        </div>
                                    </div>

                                </div>


<h3 class="MenuHeadLine">Informations ----</h3>
    <div class="menuLink">
        <div class="d-flex justify-content-between">

            <router-link :to="{name:'bankAccount'}" class="iconTex text-center">
                <i class="fa-solid fa-money-bill-transfer text-danger mx-2"></i>
                <span>Bank  <br/>Account</span>
            </router-link>

            <router-link :to="{name:'teamMember'}" class="iconTex text-center">
                <i class="fa-solid fa-chart-line text-success mx-2"></i>
                <span>Team <br/>Report</span>
            </router-link>

            <router-link :to="{name:'invite'}" class="iconTex text-center">
                <i class="fa-solid fa-square-share-nodes text-primary mx-2"></i>
                <span>Invite <br/>Friend</span>
            </router-link>



        </div>
    </div>


    <h3 class="MenuHeadLine">Reports ----</h3>

    <div class="menuLink">
        <div class="d-flex justify-content-between">

            <router-link :to="{name:'orders'}" class="iconTex text-center">
                <i class="fa-solid fa-chart-line text-success mx-2"></i>
                <span>Records</span>
            </router-link>

            <router-link :to="{name:'rechargeHistory'}" class="iconTex text-center">
                <i class="fa-solid fa-money-bill-transfer text-danger mx-2"></i>
                <span>Topup <br/>History</span>
            </router-link>

            <router-link :to="{name:'WithdrawHistory'}" class="iconTex text-center">
                <i class="fa-solid fa-money-bill-transfer text-danger mx-2"></i>
                <span>Cash Out <br/>History</span>
            </router-link>



        </div>
    </div>
    <hr/>

    <router-link :to="{name:'logout'}" class="LogoutBtn"><i class="fa-solid fa-arrow-right-from-bracket text-warning mx-2"></i> Log Out </router-link>





                                <!-- <ul data-v-7b9eb5e9="" class="list-group">

                                    <li data-v-7b9eb5e9="" class="list-group-item">
                                        <router-link :to="{name:'teamMember'}" class=""><i data-v-7b9eb5e9="" class="fa-solid fa-chart-line text-success mx-2"></i> Team Report </router-link>
                                    </li>

                                    <li data-v-7b9eb5e9="" class="list-group-item">
                                        <router-link :to="{name:'bankAccount'}" class=""><i data-v-7b9eb5e9="" class="fa-solid fa-money-bill-transfer text-danger mx-2"></i>Bank Account </router-link>
                                    </li>

                                    <li data-v-7b9eb5e9="" class="list-group-item">
                                        <router-link :to="{name:'rechargeHistory'}" class=""><i data-v-7b9eb5e9="" class="fa-solid fa-money-bill-transfer text-danger mx-2"></i>Topup History </router-link>
                                    </li>

                                    <li data-v-7b9eb5e9="" class="list-group-item">
                                        <router-link :to="{name:'WithdrawHistory'}" class=""><i data-v-7b9eb5e9="" class="fa-solid fa-money-bill-transfer text-danger mx-2"></i>Cash Out History </router-link>
                                    </li>
                                    <li data-v-7b9eb5e9="" class="list-group-item">
                                        <router-link :to="{name:'invite'}" class=""><i data-v-7b9eb5e9="" class="fa-solid fa-square-share-nodes text-primary mx-2"></i> Invite Friend </router-link>
                                    </li>

                                    <li data-v-7b9eb5e9="" class="list-group-item">
                                        <a data-v-7b9eb5e9="" :href="$asseturl+'_DMMART_16520202.apk'"><i data-v-7b9eb5e9="" class="fa-solid fa-cloud-arrow-down mx-2"></i> App Download Link </a>
                                    </li>

                                    <li data-v-7b9eb5e9="" class="list-group-item" style="padding-bottom: 2rem;">
                                        <router-link :to="{name:'logout'}"><i data-v-7b9eb5e9="" class="fa-solid fa-arrow-right-from-bracket text-warning mx-2"></i> Log Out </router-link>
                                    </li>
                                </ul> -->
                            </div>
                        </div>



    </div>
</template>
<script>

import { ButtonCopy,ButtonTelegram  } from 'share-button-links/components/buttons';
export default {
    components:{
        ButtonCopy,ButtonTelegram
    },
    data(){
        return {
            settings:{},
              row: {
                plans:{},
                deposit:{},
                depositamount:0,
                user:{},
                withdraw:{},
                withdrawamount:0,
                refercount:0,
            },
        }
    },
    methods: {
          async getData() {



            var resN = await this.callApi('get',`/api/admin/setting`,[])
              this.settings = resN.data

             var id = localStorage.getItem('userid');
            var res = await this.callApi('get', `/api/admin/user/${id}`, []);
            this.row = res.data;

        },



    },
    mounted() {
            this.getData();

    },
}
</script>

<style scoped>
a.LogoutBtn {
    width: 100%;
    display: block;
    padding: 8px 5px;
    border: 1px solid #b3b3b3;
    text-align: center;
    background: #0077C3;
    color: white;
    text-decoration: none;
}

a.iconTex.text-center {
    border: 1px solid #b9b9b9;
    padding: 8px 6px;
    width: 85px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: #0077C3;
    text-decoration: none;
    font-weight: 500;
    font-size: 12px;
}

a.iconTex.text-center i {



    font-size: 35px;
}

.MenuHeadLine{
    border-bottom: 1px solid #646464;
    padding: 10px 0px;
    color: #646464;
}
.inviteButton{
    border-radius: 0px 40px;
    border: 1px solid #ff2323;
    padding: 4px 17px;
    font-size: 16px;
    font-weight: 600;
    margin-top: 10px;
}
.profileLinks i {
    font-size: 31px;
    padding: 10px;
}
.profileLinks {
    font-size: 12px;
    color: white;
    margin: 14px 3px;
}
section.accontDetails {
    background: #008dff;
    color: white;
    padding: 32px 16px;
    margin-top: -40px;
}

a.accountList {
    color: white !important;
}

a.accountList.odd {
    background: #003cff !important;
}

a.accountList.even {
    background: #af5016 !important;
}



/*
a.accountList.listCompanny {
    background: #af1616 !important;
}

a.accountList.listInformaion {}

a.accountList.listInformaion {
    background: #af165b !important;
}

a.accountList.listorder {
    background: #9516af !important;
}

a.accountList.listReHis {
    background: #5616af !important;
}

a.accountList.listWithHis {
    background: #2716af !important;
}

a.accountList.listInvite {
    background: #1653af !important;
}

a.accountList.listCus1 {
    background: #16af56 !important;
}

a.accountList.listTeleGroup {
    background: #1692af !important;
}

a.accountList.listCus2 {
    background: #82af16 !important;
}




a.accountList.listCompanny:hover {
    background: #d51919 !important;
}



a.accountList.listInformaion:hover {
    background: #d7186e !important;
}

a.accountList.listorder:hover {
    background: #bd1cde !important;
}

a.accountList.listReHis:hover {
    background: #6719d4 !important;
}

a.accountList.listWithHis:hover {
    background: #2f17e2 !important;
}

a.accountList.listInvite:hover {
    background: #1c69dc !important;
}

a.accountList.listCus1:hover {
    background: #19d969 !important;
}

a.accountList.listTeleGroup:hover {
    background: #1ab3d5 !important;
}

a.accountList.listCus2:hover {
    background: #97cc1a !important;
} */




</style>
