<template>
    <div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="/">홈</b-navbar-brand>
                <Sidebar/>

    <b-collapse id="nav-collapse" is-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="검색어"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">검색</b-button>
        </b-nav-form>


        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template #button-content>
            <em>사용자</em>
          </template>
          <b-dropdown-item href="#">개인정보</b-dropdown-item>
          <b-dropdown-item href="#">내 게시물</b-dropdown-item>
          <b-dropdown-item href="#">로그아웃</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>


<script>
  import Sidebar from '@/components/Sidebar'
  
  export default {
    components:{
      Sidebar
    }
  }
</script>