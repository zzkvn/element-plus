<template>
  <el-dropdown trigger="click" @command="handleCommand">
    <el-button type="primary">
      导出风险<i class="el-icon-arrow-down el-icon--right"></i>
    </el-button>
    <el-dropdown-menu slot="dropdown">
      <el-dropdown-item command="advancedExport">高级导出</el-dropdown-item>
    </el-dropdown-menu>
  </el-dropdown>
</template>

<script>
export default {
  methods: {
    handleCommand(command) {
      if (command === 'advancedExport') {
        // 处理高级导出的逻辑
        this.handleAdvancedExport();
      }
    },
    handleAdvancedExport() {
      // 这里写高级导出的逻辑
      console.log('执行高级导出');
    }
  }
};
</script>


<script setup lang="ts">
import {
  ArrowLeft,
  ArrowRight,
  Delete,
  Edit,
  Share,
} from '@element-plus/icons-vue'
</script>
